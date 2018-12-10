# Broadcam Wifi Driver Installing For Linux Guide
How to install the Broadcam Wifi driver on a linux system. Made for myself as a guide after installing linux on an old Windows Vista Compaq Presario CQ40.

1) Download [this file](http://mirrors.kernel.org/ubuntu/pool/main/b/b43-fwcutter/b43-fwcutter_015-9_amd64.deb) and [this file](http://www.lwfinger.com/b43-firmware/broadcom-wl-5.100.138.tar.bz2)

2) In the terminal run: (files places in Home directory)
-```
sudo dpkg -i b43-fwcutter_015-9_amd64.deb
tar xfvj broadcom-wl-5.100.138.tar.bz2
sudo b43-fwcutter -w /lib/firmware broadcom-wl-5.100.138/linux/wl_apsta.o
sudo modprobe b43
```

[Source](https://askubuntu.com/questions/730799/installing-firmware-b43-installer-offline/730813#730813)
