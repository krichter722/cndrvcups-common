dnl Process this file with autoconf to produce a configure script.

AC_INIT([cngplp], [0.1], [krichter722@aol.de])
AC_CONFIG_MACRO_DIR([m4])
LT_INIT
AM_INIT_AUTOMAKE([foreign])
AM_CONFIG_HEADER(config.h)
AM_MAINTAINER_MODE

AC_ISC_POSIX
AC_PROG_CC
AM_PROG_CC_STDC
AC_HEADER_STDC
AM_PROG_LIBTOOL

pkg_modules="gtk+-2.0 >= 2.0.0"
PKG_CHECK_MODULES(PACKAGE, [$pkg_modules])
AC_SUBST(PACKAGE_CFLAGS)
AC_SUBST(PACKAGE_LIBS)

libglade_modules="libglade-2.0 >= 2.0.0"
PKG_CHECK_MODULES(GLADE_PACKAGE,[$libglade_modules])
AC_SUBST(GLADE_PACKAGE_CFLAGS)
AC_SUBST(GLADE_PACKAGE_LIBS)

GETTEXT_PACKAGE=cngplp
AC_SUBST(GETTEXT_PACKAGE)
AC_DEFINE_UNQUOTED(GETTEXT_PACKAGE,"$GETTEXT_PACKAGE", [Gettext package.])

dnl Add the languages which your application supports here.
ALL_LINGUAS="ja fr it de es"
AM_GLIB_GNU_GETTEXT

AC_PROG_LIBTOOL

AC_CONFIG_FILES([Makefile
cnjatool/Makefile
src/Makefile
po/Makefile])
AC_OUTPUT

