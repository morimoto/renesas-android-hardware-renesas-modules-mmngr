CFILES = mmngr_buf_drv.c

obj-m += mmngrbuf.o
mmngrbuf-objs := $(CFILES:.c=.o)

ccflags-y	+= -I$(PWD)/../include

all:
	make -C $(KERNELDIR) M=$(PWD) modules
clean:
	make -C $(KERNELDIR) M=$(PWD) clean

