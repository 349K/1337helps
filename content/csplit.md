# csplit command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: csplit [OPTION]... FILE PATTERN...
Output pieces of FILE separated by PATTERN(s) to files 'xx00', 'xx01', ...,
and output byte counts of each piece to standard output.

Read standard input if FILE is -

Mandatory arguments to long options are mandatory for short options too.
  -b, --suffix-format=FORMAT  use sprintf FORMAT instead of %02d
  -f, --prefix=PREFIX        use PREFIX instead of 'xx'
  -k, --keep-files           do not remove output files on errors
      --suppress-matched     suppress the lines matching PATTERN
  -n, --digits=DIGITS        use specified number of digits instead of 2
  -s, --quiet, --silent      do not print counts of output file sizes
  -z, --elide-empty-files    remove empty output files
      --help     display this help and exit
      --version  output version information and exit

Each PATTERN may be:
  INTEGER            copy up to but not including specified line number
  /REGEXP/[OFFSET]   copy up to but not including a matching line
  %REGEXP%[OFFSET]   skip to, but not including a matching line
  {INTEGER}          repeat the previous pattern specified number of times
  {*}                repeat the previous pattern as many times as possible

A line OFFSET is a required '+' or '-' followed by a positive integer.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Full documentation at: <http://www.gnu.org/software/coreutils/csplit>
or available locally via: info '(coreutils) csplit invocation'

~~~