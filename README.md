# Odroid UPS kit for M1S firmware (CH552-based), forked from original Hardkernel's rev 0.6.

This repo attempts to maintain an updated version of the [UPS kit for M1S](https://wiki.odroid.com/accessory/power_supply_battery/m1s_ups) firmware, with non exhaustive aims:

- Modern PlatformIO development framework support
- Example implementation of CH55x-based project with ch55xduino framework in PlatformIO
- Fixes & enhancements
- External contributions

## Build

```shell
pio run -e release
```

## Upload

The recommanded method to update CH552 MCU firmware is through [Hardkernel upstream guide](https://wiki.odroid.com/accessory/power_supply_battery/m1s_ups#how_to_update_ups_firmware). They ship a recent ARM64 version of `vnproch55x` flashing tool to run on the M1S.

```shell
/path/to/fw_update.sh .pio/build/release/firmware.hex
```
