## Process this file with automake to produce Makefile.in

TESTS = check_roman_math
check_PROGRAMS = check_roman_math
check_roman_math_SOURCES = check_roman_math.c $(top_builddir)/src/roman_math.h
check_roman_math_CFLAGS = @CHECK_CFLAGS@
check_roman_math_LDADD = $(top_builddir)/src/libroman_math.la @CHECK_LIBS@
