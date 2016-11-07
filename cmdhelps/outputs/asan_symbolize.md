# asan_symbolize command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: asan_symbolize [-h] [-d] [-s SYSROOT] [-c CROSS_COMPILE] [-l LOGFILE]
                      [path_to_cut [path_to_cut ...]]

ASan symbolization script

positional arguments:
  path_to_cut           pattern to be cut from the result file path

optional arguments:
  -h, --help            show this help message and exit
  -d, --demangle        demangle function names
  -s SYSROOT            set path to sysroot for sanitized binaries
  -c CROSS_COMPILE      set prefix for binutils
  -l LOGFILE, --logfile LOGFILE
                        set log file name to parse, default is stdin

Example of use:
  asan_symbolize.py -c "$HOME/opt/cross/bin/arm-linux-gnueabi-" -s "$HOME/SymbolFiles" < asan.log

~~~
