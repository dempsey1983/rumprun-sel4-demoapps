#
# Copyright 2017, Data61
# Commonwealth Scientific and Industrial Research Organisation (CSIRO)
# ABN 41 687 119 230.
# This software may be distributed and modified according to the terms of
# the BSD 2-Clause license. Note that NO WARRANTY is provided.
# See "LICENSE_BSD2.txt" for details.
# @TAG(DATA61_BSD)
#

ARCHIVE = redis
BAKE_TARGET = $(PROJECT_BASE)/projects/rumprun-packages/redis/bin/redis-server
PATH2 := ${PATH}

include $(PROJECT_BASE)/apps/rumpcommon.mk

.PHONY: $(BAKE_TARGET)_
$(BAKE_TARGET)_:
	cd $(PROJECT_BASE)/projects/rumprun-packages/redis && \
	env -i PATH=${PATH2} RUMPRUN_TOOLCHAIN_TUPLE=$(RRTOOLCHAIN) make cache
