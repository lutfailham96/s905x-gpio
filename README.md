# s905x-gpio
GPIO controller for Amlogic S905X devices

## Instalation
- choose your s905x device model, example for model ```hg680p```
- install gpio controller to system
```sh
(cd /usr/bin && curl -sLko hg680p.sh https://raw.githubusercontent.com/lutfailham96/s905x-gpio/main/hg680p.sh && chmod +x hg680p.sh)
```
- run ```device_model.sh``` script to show help menu
```sh
hg680p.sh
```
output:
```sh
Usage:
  -power  [on, off, warn, dis]
  -lan    [on, off, warn, dis]
  -usb    [reset]
```

## Resetting USB Devices
- some s905x gpio controller contains feature to reset USB device such as ```hg680p```
- to reset USB devices, simply type command:
```sh
hg680p.sh -usb reset
```
