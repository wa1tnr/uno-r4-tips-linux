Sun  9 Jul 13:49:13 UTC 2023


# uno-r4-tips-linux

## arduino-cli-uno-r4

 * udev rules a must for Linux

```
cat /etc/udev/rules.d/60-arduino-renesas.rules 

# Renesas based Arduino Santiago/Portenta H33 bootloader mode UDEV rules

SUBSYSTEMS=="usb", ATTRS{idVendor}=="2341", MODE:="0666"
```

 * arduino-cli installs this when run as root - not good
 * discovery made with Uno R4 Minima not Uno R4 WiFi
 * minima model requires this
 * wifi model does not!
 * wifi model uses ESP32 to interface with host PC USB
 * minima model uses 'something else' (the RA4M1 chip, itself, most likely: TODO find out)

**Sun  9 Jul 14:14:35 UTC 2023**
**END.**
