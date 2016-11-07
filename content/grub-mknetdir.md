# grub-mknetdir command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: grub-mknetdir [OPTION...]

      --compress[=no,xz,gz,lzo]   compress GRUB files [optional]
  -d, --directory=DIR        use images and modules under DIR
                             [default=/usr/lib/grub/<platform>]
      --fonts=FONTS          install FONTS [default=unicode]
      --install-modules=MODULES   install only MODULES and their dependencies
                             [default=all]
  -k, --pubkey=FILE          embed FILE as public key for signature checking
      --locale-directory=DIR use translations under DIR
                             [default=/usr/share/locale]
      --locales=LOCALES      install only LOCALES [default=all]
      --modules=MODULES      pre-load specified modules MODULES
      --themes=THEMES        install THEMES [default=starfield]
  -v, --verbose              print verbose messages.
      --core-compress=xz|none|auto
                             choose the compression to use for core image
      --net-directory=DIR    root directory of TFTP server
      --subdir=DIR           relative subdirectory on network server
  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Prepares GRUB network boot images at net_directory/subdir assuming
net_directory being TFTP root.

Report bugs to <bug-grub@gnu.org>.

~~~
