AC_INIT([cnusb], [1.0.0], [krichter722@aol.de])
AC_CONFIG_MACRO_DIR([m4])
LT_INIT
AM_INIT_AUTOMAKE([foreign])
AM_CONFIG_HEADER(config.h)

AC_ARG_ENABLE(progpath)
if test "${enable_progpath}" = "" ; then
   enable_progpath="$prefix/bin"
fi

AC_DEFINE_UNQUOTED(PROG_PATH, "$enable_progpath")
AC_SUBST(PROG_PATH)

# Checks for programs.
AC_PROG_CC

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([fcntl.h stdlib.h sys/ioctl.h termios.h])

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.
AC_PROG_GCC_TRADITIONAL
AC_FUNC_SELECT_ARGTYPES
AC_TYPE_SIGNAL
AC_FUNC_VPRINTF
AC_CHECK_FUNCS([memmove memset select strchr strerror strncasecmp strstr])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
