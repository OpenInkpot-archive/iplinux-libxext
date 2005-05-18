#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.57)
AC_INIT([libXext],
        6.4.3,
        [keithp@keithp.com],
        libXext)

AC_CONFIG_SRCDIR([Makefile.am])
AM_INIT_AUTOMAKE([dist-bzip2])

AM_MAINTAINER_MODE

AM_CONFIG_HEADER([config.h])

# Checks for programs.
AC_PROG_LIBTOOL
AC_PROG_CC

# Checks for pkg-config packages
PKG_CHECK_MODULES(XEXT, xproto x11 xextproto)
AC_SUBST(XEXT_CFLAGS)
AC_SUBST(XEXT_LIBS)

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC

AC_OUTPUT([Makefile
           man/Makefile
	   src/Makefile
	   xext.pc])