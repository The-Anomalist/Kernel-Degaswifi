#
# Makefile for the drivers of Marvell devices.
#
ifdef CONFIG_TZ_HYPERVISOR
obj-y				+= security/mmp-tzdd/src/
else
obj-y				+= security/mmp-geu/
endif
ifeq ($(BOARD_GFX_DRIVER_VERSION),)
  BOARD_GFX_DRIVER_VERSION := 4x
endif
obj-$(CONFIG_MRVL_GPU_GALCORE)	+= graphics/galcore_$(BOARD_GFX_DRIVER_VERSION)/
obj-$(CONFIG_MRVL_MMP_MODEM)	+= marvell-telephony/

obj-$(CONFIG_MRVL_WL_SD8887) += sd8887/
obj-$(CONFIG_MRVL_WL_SD8777) += sd8777/
obj-$(CONFIG_MRVL_WL_SD8787) += sd8787/
obj-$(CONFIG_MRVL_WL_SD8897) += sd8897/
obj-$(CONFIG_MRVL_WL_SD8XXX) += sd8777/ sd8787/ sd8887/ sd8897/