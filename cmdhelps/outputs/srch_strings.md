# srch_strings command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: srch_strings [option(s)] [file(s)]
 Display printable strings in [file(s)] (stdin by default)
 The options are:
  -a -                 Scan the entire file, not just the data section
  -f       Print the name of the file before each string
  -n number       Locate & print any NUL-terminated sequence of at
  -<number>                 least [number] characters (default 4).
  -t {o,x,d}        Print the location of the string in base 8, 10 or 16
  -o                        An alias for --radix=o
  -e {s,S,b,l,B,L} Select character size and endianness:
                            s = 7-bit, S = 8-bit, {b,l} = 16-bit, {B,L} = 32-bit
  -h                  Display this information
  -v               Print the program's version number

~~~
