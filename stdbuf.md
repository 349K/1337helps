# stdbuf command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: stdbuf OPTION... COMMAND
Run COMMAND, with modified buffering operations for its standard streams.

Mandatory arguments to long options are mandatory for short options too.
  -i, --input=MODE   adjust standard input stream buffering
  -o, --output=MODE  adjust standard output stream buffering
  -e, --error=MODE   adjust standard error stream buffering
      --help     display this help and exit
      --version  output version information and exit

If MODE is 'L' the corresponding stream will be line buffered.
This option is invalid with standard input.

If MODE is '0' the corresponding stream will be unbuffered.

Otherwise MODE is a number which may be followed by one of the following:
KB 1000, K 1024, MB 1000*1000, M 1024*1024, and so on for G, T, P, E, Z, Y.
In this case the corresponding stream will be fully buffered with the buffer
size set to MODE bytes.

NOTE: If COMMAND adjusts the buffering of its standard streams ('tee' does
for example) then that will override corresponding changes by 'stdbuf'.
Also some filters (like 'dd' and 'cat' etc.) don't use streams for I/O,
and are thus unaffected by 'stdbuf' settings.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Full documentation at: <http://www.gnu.org/software/coreutils/stdbuf>
or available locally via: info '(coreutils) stdbuf invocation'

~~~
