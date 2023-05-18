# Bash

Stabilize shell:

`python -c 'import pty;pty.spawn("/bin/bash/")'`

Spawn a process, and connect its controlling terminal with the current process’s standard io. This is often used to baffle programs which insist on reading from the controlling terminal.

|      Command      |             Full name             |            Purpose           |
| :---------------: | :-------------------------------: | :--------------------------: |
|       touch       |               touch               |          create file         |
|       mkdir       |           make directory          |        create a folder       |
|         cp        |                copy               |     copy a file or folder    |
|         mv        |                move               |     move a file or folder    |
|         rm        |               remove              |    remove a file or folder   |
|        file       |                file               | determine the type of a file |
|       man ls      |             manual ls             |           manual ls          |
|       ls -a       |     list files and directories    |        list all files        |
|     su -user2     |            switch user            |        switch to user2       |
|        PID        |   process identification number   |        PID process ID        |
|       ps aux      | snapshot of the current processes |       running processes      |
| Find . -name ‘\*’ |               find                |       shows all folders      |

**ctrl + shift + c** - copy text

**ctrl + shift + v** - past text

**ctrl + a** - jumps to the beginning of line

**ctrl + e** - jumps to the end of line

**ctrl + shift + "+"** - zoom in

**ctrl + "-"** - zoom out

**ctrl + u** - deletes everything before cursor

**ctrl + k** - deletes everything after cursor

**ctrl + y** - put it back

**alt + backspace** - delete lasr word

**ctrl + x + e** - put line into editor

**ctrl + r** - find command in history



systemctl => this command allows us to interact with the systemd process/daemon.

systemctl \[option] \[service] We can do four options with systemctl:

* Start
* Stop
* Enable
* Disable

How to stop process:

`ctrl+c`

`ctrl+z` - sleep

`jobs` - find what jobs are sleeping

`bg 1` - background process

`fg 1` - back to foreground&#x20;

`wc` - word count

Found what processes is running with `jobs` and `ps` and then:

`kill -2 21345`

`pkill -9 ping kill` all ping processes

`[[ 12 =~ [0-9]+$ ]] && echo yes` - test bash script in command line

`HISTSIZE 500` - set size of history



Save IP address:

`export IP=10.10.120.2`

then:

`$IP`



* cmd+d => split terminal into 2
* shif+cmd+d => undo split
* ctrl+z => background a process
* fg => bring the process back to focus screen
* sigterm => kill the process, but allow it to do some cleanup tasks beforehand
* sigkill => kill the process, doesn't do any cleanup tasks
* sigstop => stop/ susspend a process kill
* ping google.com
* traceroute google.com => map the path your request takes as it heads to the target machine
* whois google.com => info about google IP
* nc => telnet find which port is open
* pdfinfo exiftool
* **`curl -s google.com`**
* `curl -s http://10.10.10.10/whatever`
* `echo -n "neco==" | base64 -d`

`http -v GET https://949e28ad57a200b65ef6eeb47841e4d8.ctf.hacker101.com/s3cr3t-4dm1n/ X-Forwarded-For:8.8.8.8`

using redirection: `<command> < <file_name>`

There’s two types of output, `stdout` (standard out) for when a command is successful, and `stderr` (standard error) for when it’s not.

You can redirect `stderr` with `2>`

use `1>` to redirect `stdout`

`stdin` (standard in) is the third thing commands can use and is for getting input.&#x20;

&#x20;you can redirect `stdin` as well. Here's an example: `<command> < <filename_for_stdin>`

&#x20;Another way to set the `stdin` is by using the pipe (`|`). It will use the output from one command as input for another. Here's an example: `<command_1> | <command_2>`. This will take the `stdout` from `command_1` and use it as the `stdin` for `command_2`.&#x20;



Settings stuff:

Global:

/etc/profile

/etc/bashrc



Users:

\~/.bash\_profile

\~/.bashrc

\~/.bash\_logout

\~/.bash\_history



## Raspberry Pi

`cd LCD-show/`

`./LCD35B-show-v2`

change to HDMI

`cd LCD-show/`

`./LCD-hdmi`

### Start the SSH service with `systemctl`

> ```
> sudo systemctl enable ssh
> sudo systemctl start ssh
> ```

#### Wifi Router

`sudo apt install hostapd`

`sudo apt install dnsmasq`

`sudo DEBIAN_FRONTEND=noninteractive apt install -y netfilter-persistent iptables-persistent`

Setting AP (Access Point)

First remove it:

`sudo systemctl unmask hostapd.service`

Then enable it:

`sudo systemctl enable hostapd.service`

Need to delete to get back with wifi connection:

`sudo nano /etc/dhcpcd.conf`

```
interface wlan0
           static ip_address=10.20.1.1/24
           nohook wpa_supplicant
```

`sudo nano /etc/sysctl.d/router-ap.conf`

&#x20;    net.ipv4.ip\_forward=1

`sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE`

`sudo netfilter-persistent save`

`sudo mv /etc/dnsmasq.conf /etc/dnsmasq.conf.old`

`sudo touch /etc/dnsmasq.conf`

```
interface=wlan0
dhcp-range=10.20.1.5,10.20.1.100,255.255.255.0,72h
domain=wlan
address=/rt.wlan/10.20.1.1
```

`sudo touch /etc/hostapd/hostapd.conf`

`sudo nano /etc/hostapd/hostapd.conf`

```
country_code=CZ
interface=wlan0
ssid=RaspberryPiWiFi
hw_mode=a
channel=36
macaddr_acl=0
auth_algs=1
ignore_broadcast_ssid=0
wpa=2
wpa_passphrase=RaspberryPassword
wpa_key_mgmt=WPA-PSK
wpa_pairwise=TKIP
rsn_pairwise=CCMP
```

`sudo reboot`

#### Try it different

#### 1. Install and update Raspbian

`sudo apt-get update`

`sudo apt-get upgrade`

#### 2. Install hostapd and dnsmasq

`sudo apt-get install hostapd`

`sudo apt-get install dnsmasq`

`sudo systemctl stop hostapd`

`sudo systemctl stop dnsmasq`

#### 3. Configure a static IP for the wlan0 interface

`sudo nano /etc/dhcpcd.conf`

Write in:

```
interface wlan0
static ip_address=192.168.4.1/24
interface eth0
static ip_address=192.168.4.2/24

denyinterfaces eth0
denyinterfaces wlan0
```

#### 4. Configure the DHCP server (dnsmasq)

`sudo mv /etc/dnsmasq.conf /etc/dnsmasq.conf.orig`

`sudo nano /etc/dnsmasq.conf`

Write in:

```
interface=wlan0
dhcp-range=192.168.4.10,192.168.4.100,255.255.255.0,72h
```

#### 5. Configure the access point host software (hostapd)

`sudo nano /etc/hostapd/hostapd.conf`

```
interface=wlan0
bridge=br0
hw_mode=g
channel=7
wmm_enabled=0
macaddr_acl=0
auth_algs=1
ignore_broadcast_ssid=0
wpa=2
wpa_key_mgmt=WPA-PSK
wpa_pairwise=TKIP
rsn_pairwise=CCMP
ssid=RaspberryWifi
wpa_passphrase=RPIPassword
```

`sudo nano /etc/default/hostapd`

Track this line:

`DAEMON_CONF="/etc/hostapd/hostapd.conf"`

#### 6. Set up traffic forwarding

`sudo nano /etc/sysctl.conf`

Track this line:

`net.ipv4.ip_forward=1`

#### 7. Add a new iptables rule

`sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE`

`sudo sh -c "iptables-save > /etc/iptables.ipv4.nat"`

`iptables-restore < /etc/iptables.ipv4.nat`

#### 8. Enable internet connection

`sudo apt-get install bridge-utils`

`sudo brctl addbr br0`

`sudo brctl addif br0 eth0`

`sudo nano /etc/network/interfaces`

Add following lines at the end of the file:

```
auto br0
iface br0 inet manual
bridge_ports eth0 wlan0
```

#### Reboot

`sudo reboot`

[https://raspberrypi.stackexchange.com/questions/88954/workaround-for-a-wifi-bridge-on-a-raspberry-pi-with-proxy-arp/88955#88955](https://raspberrypi.stackexchange.com/questions/88954/workaround-for-a-wifi-bridge-on-a-raspberry-pi-with-proxy-arp/88955#88955)



Check to make sure that the wlan0 interface is up and running. You can check this by running the command "ip link show wlan0". If the interface is down, you can bring it up by running the command "sudo ip link set wlan0 up".



You can check the IP address assigned to wlan0 by running the command "sudo ifconfig wlan0". It should display the IP address assigned to the wlan0 interface. If the IP address is not assigned, you can try running "sudo dhclient wlan0" to obtain an IP address from the DHCP server.

### VPN

`wg0` is a network interface for a WireGuard VPN connection.&#x20;

`tun0` is also a network interface that is used for VPN connections. It is typically used for OpenVPN connections.



Podivat se:

arp spoofing

aircraft engine

ettercap

ssl self-signed certificate

ssl stripping

