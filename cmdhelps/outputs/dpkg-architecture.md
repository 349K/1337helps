# dpkg-architecture command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-architecture [<option>...] [<command>]

Commands:
  -l, --list                list variables (default).
  -L, --list-known          list valid architectures (matching some criteria).
  -e, --equal <arch>        compare with host Debian architecture.
  -i, --is <arch-wildcard>  match against host Debian architecture.
  -q, --query <variable>    prints only the value of <variable>.
  -s, --print-set           print command to set environment variables.
  -u, --print-unset         print command to unset environment variables.
  -c, --command <command>   set environment and run the command in it.
  -?, --help                show this help message.
      --version             show the version.

Options:
  -a, --host-arch <arch>    set host Debian architecture.
  -t, --host-type <type>    set host GNU system type.
  -A, --target-arch <arch>  set target Debian architecture.
  -T, --target-type <type>  set target GNU system type.
  -W, --match-wildcard <arch-wildcard>
                            restrict architecture list matching <arch-wildcard>.
  -B, --match-bits <arch-bits>
                            restrict architecture list matching <arch-bits>.
  -E, --match-endian <arch-endian>
                            restrict architecture list matching <arch-endian>.
  -f, --force               force flag (override variables set in environment).

~~~
