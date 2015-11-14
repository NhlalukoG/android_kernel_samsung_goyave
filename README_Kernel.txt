################################################################################
HOW TO BUILD KERNEL FOR SM-T116NY_SWA

1. How to Build
	- get Toolchain
	download and install arm-eabi-4.7 toolchain for ARM EABI.
	Extract kernel source and move into the top directory.

	$ make goyave3g-dt_hw00_defconfig
	$ make -j64
	
2. Output files
	- Kernel : Kernel/arch/arm/boot/zImage
	- module : Kernel/drivers/*/*.ko
	
3. How to Clean	
    $ make clean
	
4. How to make .tar binary for downloading into target.
	- change current directory to Kernel/arch/arm/boot
	- type following command
	$ tar cvf SM-T116NY_SWA.tar zImage
#################################################################################