ARCH := arm
CROSS_COMPILE := /home/cepera/projects/learn/qemulinux/buildroot-2022.02.9/output/host/bin/arm-buildroot-linux-gnueabi-
obj-m := mymod.o
KDIR := /home/cepera/projects/learn/qemulinux/buildroot-2022.02.9/output/build/linux-5.15.18
PWD := $(shell pwd)
export

ccflags-y += -g -DDEBUG

default:
	$(MAKE) -C $(KDIR) M=$(PWD) modules
clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean

