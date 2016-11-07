# tilt command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: tilt <options> <file>
Process template <file> and write output to stdout. With no <file> or
when <file> is '-', read template from stdin and use the --type option
to determine the template's type.

Options
  -l, --list           List template engines + file patterns and exit
  -t, --type=<pattern> Use this template engine; required if no <file>
  -y, --layout=<file>  Use <file> as a layout template

  -D<name>=<value>     Define variable <name> as <value>
  --vars=<ruby>        Evaluate <ruby> to Hash and use for variables

  -h, --help           Show this help message

Convert markdown to HTML:
  $ tilt foo.markdown > foo.html

Process ERB template:
  $ echo "Answer: <%= 2 + 2 %>" | tilt -t erb
  Answer: 4

Define variables:
  $ echo "Answer: <%= 2 + n %>" | tilt -t erb --vars="{:n=>40}"
  Answer: 42
  $ echo "Answer: <%= 2 + n.to_i %>" | tilt -t erb -Dn=40
  Answer: 42

~~~
