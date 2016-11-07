# icu-config command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

icu-config: icu-config: ICU configuration helper script

The most commonly used options will be --cflags, --cxxflags, --cppflags, and --ldflags.
Example (in make):   CPFLAGS=$(shell icu-config --cppflags)
                     LDFLAGS=$(shell icu-config --ldflags)
                     (etc)..

Usage:
  --noverify             Don't verify that ICU is actually installed.
  --bindir               Print binary directory path (bin)
  --cc                   Print C compiler used [CC]
  --cflags               Print C compiler flags [CFLAGS]
  --cflags-dynamic       Print additional C flags for
                             building shared libraries.
  --cppflags             Print C Preprocessor flags [CPPFLAGS]
  --cppflags-dynamic     Print additional C Preprocessor flags for
                             building shared libraries.
  --cppflags-searchpath  Print only -I include directives  (-Iinclude)
  --cxx                  Print C++ compiler used [CXX]
  --cxxflags             Print C++ compiler flags [CXXFLAGS]
  --cxxflags-dynamic     Print additional C++ flags for
                             building shared libraries.
  --detect-prefix        Attempt to detect prefix based on PATH
  --exec-prefix          Print prefix for executables (/bin)
  --exists               Return with 0 status if ICU exists else fail
  --help, -?, --usage    Print this message
  --icudata              Print shortname of ICU data file (icudt21l)
  --icudata-install-dir  Print path to install data to - use as --install option to pkgdata(1)
  --icudata-mode         Print default ICU pkgdata mode (dll) - use as --mode option to pkgdata(1).
  --icudatadir           Print path to packaged archive data. Can set as [ICU_DATA]
  --invoke               Print commands to invoke an ICU program
  --invoke=<prog>        Print commands to invoke an ICU program named <prog> (ex: genrb)
  --ldflags              Print -L search path and -l libraries to link with ICU [LDFLAGS].  This is for the data, uc (common), and i18n libraries only.  
  --ldflags-layout       Print ICU layout engine link directive. Use in addition to --ldflags
  --ldflags-libsonly     Same as --ldflags, but only the -l directives
  --ldflags-searchpath   Print only -L (search path) directive
  --ldflags-system       Print only system libs ICU links with (-lpthread, -lm)
  --ldflags-icuio        Print ICU icuio link directive. Use in addition to --ldflags 
  --ldflags-obsolete     Print ICU obsolete link directive. Use in addition to --ldflags. (requires icuapps/obsolete to be built and installed.) 
  --mandir               Print manpage (man) path
  --prefix               Print PREFIX to icu install (/usr/local)
  --prefix=XXX           Set prefix to XXX for remainder of command
  --sbindir              Print system binary path (sbin) 
  --shared-datadir       Print shared data (share) path. This is NOT the ICU data dir.
  --shlib-c              Print the command to compile and build C shared libraries with ICU
  --shlib-cc             Print the command to compile and build C++ shared libraries with ICU
  --sysconfdir           Print system config (etc) path
  --unicode-version      Print version of Unicode data used in ICU (8.0)
  --version              Print ICU version (57.1)
  --incfile              Print path to Makefile.inc
  --incpkgdatafile       Print path to pkgdata.inc (for -O option of pkgdata)
  --install              Print path to install-sh
  --mkinstalldirs        Print path to mkinstalldirs

 [Brackets] show MAKE variable equivalents,  (parenthesis) show example output

Copyright (c) 2002-2013, International Business Machines Corporation and others. All Rights Reserved.

NOTE: Please consider using the pkg-config (.pc) files instead of icu-config.
 See: <http://userguide.icu-project.org/howtouseicu#TOC-pkg-config> 

~~~
