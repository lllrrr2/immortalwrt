include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=ipq40xx
BOARDNAME:=Qualcomm Atheros IPQ40XX
FEATURES:=squashfs fpu ramdisk
CPU_TYPE:=cortex-a7
CPU_SUBTYPE:=neon-vfpv4
SUBTARGETS:=generic chromium mikrotik

KERNEL_PATCHVER:=6.6
KERNEL_TESTING_PATCHVER:=6.12

KERNELNAME:=zImage Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-usb-dwc3-qcom \
	kmod-leds-gpio kmod-gpio-button-hotplug \
	kmod-ath10k-ct wpad-openssl \
	kmod-usb3 kmod-usb-dwc3 ath10k-firmware-qca4019-ct \
	uboot-envtools automount cpufreq

$(eval $(call BuildTarget))
