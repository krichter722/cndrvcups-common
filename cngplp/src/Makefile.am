confdir = /usr/share/cngplp

ACLOCAL_AMFLAGS = -I m4
LDFLAGS = -lgmodule-2.0

AUTOMAKE_OPTIONS=foreign
AM_CFLAGS=-O2 -Wall
bin_PROGRAMS=cngplp
AM_CPPFLAGS= \
	-DPACKAGE_DATA_DIR=\""$(datadir)"\" \
        -DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-DPACKAGE_CONFIG_DIR=\""$(confdir)/"\"\
        @PACKAGE_CFLAGS@\
        @GLADE_PACKAGE_CFLAGS@
cngplp_SOURCES= main.c mainwnd.c mainwnd.h printerinfo.c printerinfo.h load.c load.h
cngplp_LDADD=@PACKAGE_LIBS@ @GLADE_PACKAGE_LIBS@  -lcups
cngplp_LDFLAGS=-rpath $(libdir)

conf_DATA = cngplp.glade
