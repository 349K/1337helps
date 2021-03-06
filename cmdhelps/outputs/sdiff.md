# sdiff command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sdiff [OPTION]... FILE1 FILE2
Side-by-side merge of differences between FILE1 and FILE2.

Mandatory arguments to long options are mandatory for short options too.
  -o, --output=FILE            operate interactively, sending output to FILE

  -i, --ignore-case            consider upper- and lower-case to be the same
  -E, --ignore-tab-expansion   ignore changes due to tab expansion
  -Z, --ignore-trailing-space  ignore white space at line end
  -b, --ignore-space-change    ignore changes in the amount of white space
  -W, --ignore-all-space       ignore all white space
  -B, --ignore-blank-lines     ignore changes whose lines are all blank
  -I, --ignore-matching-lines=RE  ignore changes all whose lines match RE
      --strip-trailing-cr      strip trailing carriage return on input
  -a, --text                   treat all files as text

  -w, --width=NUM              output at most NUM (default 130) print columns
  -l, --left-column            output only the left column of common lines
  -s, --suppress-common-lines  do not output common lines

  -t, --expand-tabs            expand tabs to spaces in output
      --tabsize=NUM            tab stops at every NUM (default 8) print columns

  -d, --minimal                try hard to find a smaller set of changes
  -H, --speed-large-files      assume large files, many scattered small changes
      --diff-program=PROGRAM   use PROGRAM to compare files

      --help                   display this help and exit
  -v, --version                output version information and exit

If a FILE is '-', read standard input.
Exit status is 0 if inputs are the same, 1 if different, 2 if trouble.

Report bugs to: bug-diffutils@gnu.org
GNU diffutils home page: <http://www.gnu.org/software/diffutils/>
General help using GNU software: <http://www.gnu.org/gethelp/>

~~~
