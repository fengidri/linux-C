#
# Makefile for kernel test
#
PWD         := $(shell pwd)
KVERSION    := $(shell uname -r)
#KERNEL_DIR   = /usr/src/linux-headers-$(KVERSION)/
KERNEL_DIR   = /usr/lib/modules/$(KVERSION)/build
MODULE_NAME  = proc1
obj-m       := $(MODULE_NAME).o
all:
	make -C $(KERNEL_DIR) M=$(PWD) modules
clean:
	make -C $(KERNEL_DIR) M=$(PWD) clean
