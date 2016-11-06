# dpkg-parsechangelog command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-parsechangelog [<option>...]

Options:
  -l <changelog-file>      get per-version info from this file.
  -F <changelog-format>    force changelog format.
  -S, --show-field <field> show the values for <field>.
  -?, --help               show this help message.
      --version            show the version.

Parser options:
      --format <output-format>
                           set output format (defaults to 'dpkg').
      --all                include all changes.
  -s, --since <version>    include all changes later than <version>.
  -v <version>             ditto.
  -u, --until <version>    include all changes earlier than <version>.
  -f, --from <version>     include all changes equal or later than <version>.
  -t, --to <version>       include all changes up to or equal than <version>.
  -c, --count <number>     include <number> entries from the top (or tail
                             if <number> is lower than 0).
  -n <number>              ditto.
  -o, --offset <number>    change starting point for --count, counted from
                             the top (or tail if <number> is lower than 0).

~~~
