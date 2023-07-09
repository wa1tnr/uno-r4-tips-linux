Sun  9 Jul 13:49:13 UTC 2023


# uno-r4-tips-linux

## arduino-cli-uno-r4

 * udev rules a must for Linux

```
ls -1 /etc/udev/rules.d/60-arduino-renesas.rules

```
```
cat /etc/udev/rules.d/60-arduino-renesas.rules 

# Renesas based Arduino Santiago/Portenta H33 bootloader mode UDEV rules

SUBSYSTEMS=="usb", ATTRS{idVendor}=="2341", MODE:="0666"
```

 * abc
 * def

**Sun  9 Jul 14:08:10 UTC 2023**
**END.**
