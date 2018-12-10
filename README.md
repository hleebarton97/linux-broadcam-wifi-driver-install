# Broadcam Wifi Driver Installing For Linux Guide
How to install the Broadcam Wifi driver on a linux system. Made for myself as a guide after installing linux on an old Windows Vista Compaq Presario CQ40.

Download http://mirrors.kernel.org/ubuntu/pool/main/b/b43-fwcutter/b43-fwcutter_015-9_amd64.deb
         http://www.lwfinger.com/b43-firmware/broadcom-wl-5.100.138.tar.bz2
         
```
sudo dpkg -i b43-fwcutter_015-9_amd64.deb
tar xfvj broadcom-wl-5.100.138.tar.bz2
sudo b43-fwcutter -w /lib/firmware broadcom-wl-5.100.138/linux/wl_apsta.o
sudo modprobe b43
```
