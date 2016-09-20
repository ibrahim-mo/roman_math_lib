This is the "roman_math" library (libroman_math) which has two functions:

char* add_roman(const char*, const char*);
char* subtract_roman(const char*, const char*);

It was built with automake tools for Ubunto, and it uses the "check" unit testing framework.
-----
vagrant@precise64:/vagrant/roman_math_lib$ uname -a
Linux precise64 3.2.0-23-generic #36-Ubuntu SMP Tue Apr 10 20:39:51 UTC 2012 x86_64 x86_64 x86_64 GNU/Linux
-----

To test the roman_math library with the Check unit tests, type:

make check


Following if you want to build everything from scratch (or if there is an environment compatibility issue):

========================
Autotools:

You need the following programs installed on your system:
  -- Autoconf
  -- Automake
  -- Libtool
  -- Check

It is recommended to use the latest versions.

Then, do as follows:

$ autoreconf --install
$ ./configure
$ make
$ make check

Don't do "make install" unless you want to install the roman_math library.

roman_math.c and roman_math.h are built as a library.  src/main.c:main() is a
client of libroman_math.la, just as tests/check_roman_math.c:main() is a client
of libroman_math.la
========================
