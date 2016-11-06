# printf command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: printf FORMAT [ARGUMENT]...
  or:  printf OPTION
Print ARGUMENT(s) according to FORMAT, or execute according to OPTION:

      --help     display this help and exit
      --version  output version information and exit

FORMAT controls the output as in C printf.  Interpreted sequences are:

  \"      double quote
  \\      backslash
  \a      alert (BEL)
  \b      backspace
  \c      produce no further output
  \e      escape
  \f      form feed
  \n      new line
  \r      carriage return
  \t      horizontal tab
  \v      vertical tab
  \NNN    byte with octal value NNN (1 to 3 digits)
  \xHH    byte with hexadecimal value HH (1 to 2 digits)
  \uHHHH  Unicode (ISO/IEC 10646) character with hex value HHHH (4 digits)
  \UHHHHHHHH  Unicode character with hex value HHHHHHHH (8 digits)
  %%      a single %
  %b      ARGUMENT as a string with '\' escapes interpreted,
          except that octal escapes are of the form \0 or \0NNN
  %q      ARGUMENT is printed in a format that can be reused as shell input,
          escaping non-printable characters with the proposed POSIX $'' syntax.

and all C format specifications ending with one of diouxXfeEgGcs, with
ARGUMENTs converted to proper type first.  Variable widths are handled.

NOTE: your shell may have its own version of printf, which usually supersedes
the version described here.  Please refer to your shell's documentation
for details about the options it supports.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Full documentation at: <http://www.gnu.org/software/coreutils/printf>
or available locally via: info '(coreutils) printf invocation'

~~~
