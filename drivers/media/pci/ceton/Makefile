#
# Makefile for the Ceton Infinitv CableCard DVB Tuner driver. 
#

ctn91xx-objs := ctn91xx_driver.o ctn91xx_interrupt.o ctn91xx_ioctl.o \
	ctn91xx_util.o ctn91xx_event.o ctn91xx_mpeg.o ctn91xx_pci.o ctn91xx_rtp.o  \
	ctn91xx_net.o ctn91xx_reset.o \
	   \
	ctn91xx_rpc.o

obj-$(CONFIG_VIDEO_CETON) += ctn91xx.o
EXTRA_CFLAGS := -DLINUX -DUSE_PCI=1 -DUSE_LEON=0 -DHAS_MPEG_DMA=1 -DUSE_INTERNAL=0

ccflags-y += -Idrivers/media/dvb-core/ -Idrivers/media/dvb-frontends/
ccflags-y += -Idrivers/media/tuners
