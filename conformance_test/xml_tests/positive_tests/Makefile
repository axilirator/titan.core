##############################################################################
# Copyright (c) 2000-2020 Ericsson Telecom AB
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v2.0
# which accompanies this distribution, and is available at
# https://www.eclipse.org/org/documents/epl-2.0/EPL-2.0.html
#
# Contributors:
#   Kirjak, Adrien
#
# not ready
##############################################################################
#TOPDIR := ../..
#include $(TOPDIR)/Makefile.regression

#ifdef LCOV
#COVERAGE_FLAG := -C
#endif

MAKE := make

MAKECLEAN := make clean

run:
	$(TTCN3_DIR)/bin/ttcn3_makefilegen -f -t XML_tests.tpd && \
	cd bin && \
	$(MAKE) && \
	$(TTCN3_DIR)/bin/ttcn3_start XML_tests ../XML_tests.cfg && \
	cd ..

clean:
	cd bin && \
	$(MAKECLEAN) && \
	cd .. 

.PHONY: all clean run 



