dtb-$(CONFIG_MACH_EXYNOS7570_J4LTE_MEA_OPEN) := \
	exynos7570-j4lte_mea_open_00.dtb \
	exynos7570-j4lte_mea_open_01.dtb \
	exynos7570-j4lte_mea_open_02.dtb

targets += dtbs

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM64_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif
targets += $(DTB_LIST)

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := dts/*.dtb *.dtb
