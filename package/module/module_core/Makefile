################################################
#
# module_core
#
################################################
PK_CORE_MOD_NAME        := module_core
PK_CORE_MOD_VERSION     := $(CONFIG_PK_CORE_MOD_VERSION)
PK_CORE_MOD_SITE        := $(CONFIG_PK_CORE_MOD_URL)
PK_CORE_MOD_GITHUB      := $(CONFIG_PK_CORE_MOD_GITHUB)
PK_CORE_MOD_SUBNAME     :=
PK_CORE_MOD_BUILDARCH   := $(CONFIG_PK_CORE_MOD_BUILDARCH)
PK_CORE_MOD_DIR         := $(srctree)/package/module/module_core
PK_CORE_MOD_PATCH       := $(PK_CORE_MOD_DIR)/patch
PK_CORE_MOD_BSBIT       := module_core-$(PK_CORE_MOD_VERSION).bsbit
PK_CORE_MOD_OUT         :=
PK_CORE_MOD_SCRIPTS     := $(srctree)/scripts/package/package-module.sh
PK_CORE_MOD_TAR         := $(CONFIG_PK_CORE_MOD_TAR)
PK_CORE_MOD_PACKAGE     :=
PK_CORE_MOD_CONFIG      := $(CONFIG_PK_CORE_MOD_CONFIG)
SUB_TARGET                  += $(PK_CORE_MOD_DIR)/build

PK_CORE_MOD_sh = $(CONFIG_SHELL) $(PK_CORE_MOD_SCRIPTS) \
                 $1X \
                 $(PK_CORE_MOD_NAME)X \
                 $(PK_CORE_MOD_VERSION)X \
                 $(PK_CORE_MOD_SITE)X \
                 $(PK_CORE_MOD_GITHUB)X \
                 $(PK_CORE_MOD_PATCH)X \
                 $(CONFIG_LINUX_KERNEL_VERSION)X \
	         $(CONFIG_MAIN_PROJ_NAME)X \
                 $(PK_CORE_MOD_TAR)X \
                 $(CONFIG_LINUX_KERNEL_CROSS_COMPILE)X \
                 $(PK_CORE_MOD_SUBNAME)X \
                 $(CONFIG_PK_CORE_MOD_CONFIG)X \
                 $(CONFIG_PK_CORE_MOD_LIBPATH)X \
                 $(CONFIG_PK_CORE_MOD_CPPFLAGS)X \
                 $(CONFIG_PK_CORE_MOD_DPKCONFIG)X \
                 $(CONFIG_PK_CORE_MOD_CFLAGS)X \
                 $(CONFIG_PK_CORE_MOD_LDFLAGS)X \
                 $(CONFIG_PK_CORE_MOD_CXXFLAGS)X \
                 $(CONFIG_PK_CORE_MOD_ASFLAGS)X \
                 $(PK_CORE_MOD_BSBIT)X \
                 $(PK_CORE_MOD_BUILDARCH)X \
		 $(PK_CORE_MOD_CSRCFILE)X \
                 $(CONFIG_PK_CORE_MOD_SRCFILE)X \
                 $(CONFIG_PK_CORE_MOD_CSRCFILE)

$(PK_CORE_MOD_DIR)/build: FORCE
	$(Q)$(call PK_CORE_MOD_sh,$(srctree))
