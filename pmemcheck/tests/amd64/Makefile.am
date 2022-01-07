# Persistent memory checker.
# Copyright (c) 2021, Linaro Ltd.
#
# This program is free software; you can redistribute it and/or modify
# it under the terms and conditions of the GNU General Public License,
# version 2, or (at your option) any later version, as published
# by the Free Software Foundation.
#
# This program is distributed in the hope it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
# FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
# for more details.

include $(top_srcdir)/Makefile.tool-tests.am

SUBDIRS = .

dist_noinst_SCRIPTS = \
	filter_stderr

floats_CFLAGS = -mno-sse2 -g -O3

noinst_HEADERS = common.h

EXTRA_DIST = \
    floats.stderr.exp floats.vgtest \
    isa_check.stderr.exp isa_check.vgtest \
	nt_stores.stderr.exp nt_stores.vgtest \
	sse_stores.stderr.exp sse_stores.vgtest

check_PROGRAMS = \
    floats \
    isa_check \
    nt_stores \
    sse_stores
