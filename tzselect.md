# tzselect command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: tzselect [--version] [--help] [-c COORD] [-n LIMIT]
Select a time zone interactively.

Options:

  -c COORD
    Instead of asking for continent and then country and then city,
    ask for selection from time zones whose largest cities
    are closest to the location with geographical coordinates COORD.
    COORD should use ISO 6709 notation, for example, '-c +4852+00220'
    for Paris (in degrees and minutes, North and East), or
    '-c -35-058' for Buenos Aires (in degrees, South and West).

  -n LIMIT
    Display at most LIMIT locations when -c is used (default 10).

  --version
    Output version information.

  --help
    Output this help.

Report bugs to <http://www.debian.org/Bugs/>.

~~~
