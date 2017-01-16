# --------------------------------------------------------------------------------------------------
# Makefile used to build the tool to make patches
#
# Copyright (C) Sierra Wireless Inc.
# --------------------------------------------------------------------------------------------------

# ========== GENERIC BUILD RULES ============

# Tell make that the targets are not actual files.
.PHONY: mkPatch

MKPATCH_SRC = mkPatch.c $(LEGATO_ROOT)/framework/c/src/crc.c

mkPatch: $(MKPATCH_SRC)
	gcc -o $(LEGATO_ROOT)/bin/$@ \
	    $(MKPATCH_SRC) \
	    -I$(LEGATO_ROOT)/framework/c/inc \
	    -I$(LEGATO_ROOT)/3rdParty/include