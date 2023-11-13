# NXP - iMX6/iMX8

Current iMX6 images support the ARMv7-A dual-lite and quad versions (ARM Cortex-A9) of the following boards:

* Cubox-i
* Wandboard
* Udoo

Current iMX8 images are experimental and do not support a specific board.

Installation is done by writing the LibreELEC \*.img file to an SD card. The boards have internal hardware identifiers so there is no need to edit `extlinux.conf` on the card. Selection of the correct device dtb is handled internally within U-Boot.

**NOTE** - \*\*\*\* It is not possible to update from older LibreELEC or OpenELEC imx6.arm images to LE 11.0 as the boot configuration for LE 11.0 is different and older kernels do not support zstd compression. If you attempt an upgrade, the boot configuration of the old installation will be broken. You are advised to clean install LE 11.0 and manually restore sources and library DB files. Backups can be taken and restored, but as there is now a long time gap since LE 8.2.5 (and OE 8.0.x) it is best to start over with a clean system.
