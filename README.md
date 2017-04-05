# Huawei Honor 3C (h30u10) kernel sources

## Prerequisites

	# sudo apt-get install build-essential
[arm-linux-androideabi-4.9](https://android.googlesource.com/platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/+archive/master.tar.gz)

## Build

	# export ARCH=arm && export ARCH_MTK_PLATFORM=mt6582 && export TARGET_PRODUCT=huawei82_cwet_kk
	# export CROSS_COMPILE=/PATH-TO-YOUR-TOOLCHAIN/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-

Start build:

	# ./mk r k

Append MTK headers:

	# mediatek/build/tools/mkimage out/target/product/${TARGET_PRODUCT}/obj/KERNEL_OBJ/arch/arm/boot/zImage KERNEL > ./zImage
