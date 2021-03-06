#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.65])
AC_INIT([widl],[1.0],[mingw-w64-public@lists.sourceforge.net])
AC_CONFIG_AUX_DIR([../build-aux])
AC_CONFIG_SRCDIR([src/widl.c])
AC_CONFIG_HEADERS([include/config.h])

AM_INIT_AUTOMAKE([foreign subdir-objects])
AM_MAINTAINER_MODE

AC_CANONICAL_HOST

# Checks for programs.
AC_PROG_CC

case $host in
  *-mingw32)
    widl_bin_name=widl
    CFLAGS="$CFLAGS -Wno-pedantic-ms-format"
    ;;
  *)
    widl_bin_name=mingw-w64-widl
    ;;
esac

AC_SUBST(WIDL_BIN_NAME,[$widl_bin_name])

# Checks for libraries.

# Checks for header files.
AC_CHECK_HEADERS([getopt.h io.h fcntl.h inttypes.h libintl.h limits.h malloc.h stddef.h stdlib.h string.h sys/time.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT8_T
AC_TYPE_OFF_T
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT8_T

AC_CHECK_TYPES([long long])

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_FUNC_STRTOD
AC_CHECK_FUNCS([atexit gettimeofday memmove memset mkstemp strcasecmp strchr strdup strerror strncasecmp strrchr strtol strtoul strtoull])

AH_TOP([#define __WINE_CONFIG_H])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
