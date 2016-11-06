# grub-syslinux2cfg command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: grub-syslinux2cfg [OPTION...] FILE
Transform syslinux config into GRUB one.

  -c, --cwd=DIR              current directory of the syslinux [default is
                             parent directory of input file].
  -i, --isolinux             assume input is an isolinux configuration file.
  -o, --output=FILE          write output to FILE [default=stdout].
  -p, --pxelinux             assume input is a pxelinux configuration file.
  -r, --root=DIR             root directory of the syslinux disk [default=/].
  -s, --syslinux             assume input is a syslinux configuration file.
  -t, --target-root=DIR      root directory as it will be seen on runtime
                             [default=/].
  -T, --target-cwd=DIR       current directory of the syslinux as it will be
                             seen on runtime  [default is parent directory of
                             input file].
  -v, --verbose              print verbose messages.
  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Report bugs to <bug-grub@gnu.org>.

~~~
