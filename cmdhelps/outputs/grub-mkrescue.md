# grub-mkrescue command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: grub-mkrescue [OPTION...] [OPTION] SOURCE...
Make GRUB CD-ROM, disk, pendrive and floppy bootable image.

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
      --arcs-boot            enable ARCS (big-endian mips machines, mostly
                             SGI) boot. Disables HFS+, APM, sparc64 and boot
                             as disk image for i386-pc
      --core-compress=xz|none|auto
                             choose the compression to use for core image
      --label-bgcolor=COLOR  use COLOR for label background
      --label-color=COLOR    use COLOR for label
      --label-font=FILE      use FILE as font for label
  -o, --output=FILE          save output in FILE [required]
      --product-name=STRING  use STRING as product name
      --product-version=STRING   use STRING as product version
      --rom-directory=DIR    save ROM images in DIR [optional]
      --sparc-boot           enable sparc boot. Disables HFS+, APM, ARCS and
                             boot as disk image for i386-pc
      --xorriso=FILE         use FILE as xorriso [optional]
  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Generates a bootable CD/USB/floppy image.  Arguments other than options to
this program are passed to xorriso, and indicate source files, source
directories, or any of the mkisofs options listed by the output of `xorriso
-as mkisofs -help'.

Option -- switches to native xorriso command mode.

Mail xorriso support requests to <bug-xorriso@gnu.org>.

Report bugs to <bug-grub@gnu.org>.

~~~
