CFILES = mmngr_drv.c

obj-m += mmngr.o
mmngr-objs := $(CFILES:.c=.o)

ccflags-y	+= -D$(MMNGR_CONFIG)
ccflags-y	+= -D$(MMNGR_SSP_CONFIG)
ccflags-y	+= -D$(MMNGR_IPMMU_MMU_CONFIG)
ccflags-y	+= -I$(PWD)/../include

all:
	make -C $(KERNELDIR) M=$(PWD) modules
clean:
	make -C $(KERNELDIR) M=$(PWD) clean
