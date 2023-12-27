
``` bash
sudoedit /etc/udev/rules.d/99-via.rules  
> KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0666", TAG+="uaccess", TAG+="udev-acl"  
udevadm control --reload  
sudo chown $USER:$USER /dev/hidraw*
```