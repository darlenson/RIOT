# define the module that is build
MODULE = cpu

# add a list of subdirectories, that should also be build
DIRS = periph $(CORTEX_COMMON)

# build one of the radio drivers, if enabled
ifneq (,$(filter radio_nrfmin,$(USEMODULE)))
    DIRS += radio/nrfmin
endif

include $(RIOTBASE)/Makefile.base
