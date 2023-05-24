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









