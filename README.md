# linux-5.7-h6-mainline
Linux kernel config and patches for Generic H6 tvbox( Tanix TX6 , T95 MAX and posible others) based on Allwinner H6 CPU

_Thank you guys from linux-sunxi mail-list and linux-sunxi portal with CPU documentations_

to install just apply this path to 5.7-rc6 kernel `patch -p1 <./unsorted_patch_h6-tvbox_5.7-rc6.diff`
 and build with https://linux-sunxi.org/Mainline_Kernel_Howto#Kernel_Compilation this instruction for arm64.


for boot the board you must use this devicetree file:
`sun50i-h6-tanix-tx6.dtb`

works:
 * sd/mmc
 * emmc
 * ethernet (ac200)
 * wifi(xr819)
 * usb/usb3
 * i2c
 * gpio led
 * hdmi(with audio and CEC posible)
 * CPU dvfs/frequency change
 * Temperature sensors
 * GPU with opengles (possible with opencl need to test this moment)
 * IR (hardcoded tanix tx6 remote keymap)

n/a:
 * spdiff
