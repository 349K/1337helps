# grub-mkimage command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: grub-mkimage [OPTION...] [OPTION]... [MODULES]
Make a bootable image of GRUB.

  -c, --config=FILE          embed FILE as an early config
  -C, --compression=(xz|none|auto)
                             choose the compression to use for core image
  -d, --directory=DIR        use images and modules under DIR
                             [default=/usr/lib/grub/<platform>]
  -k, --pubkey=FILE          embed FILE as public key for signature checking
  -m,                              --memdisk=FILE         embed FILE as a memdisk image
Implies `-p (memdisk)/boot/grub' and overrides
                             any prefix supplied previously, but the prefix
                             itself can be overridden by later options
  -n, --note                 add NOTE segment for CHRP IEEE1275
  -o, --output=FILE          output a generated image to FILE [default=stdout]
  -O, --format=FORMAT        generate an image in FORMAT
                             available formats: i386-coreboot, i386-multiboot,
                             i386-pc, i386-pc-pxe, i386-pc-eltorito, i386-efi,
                             i386-ieee1275, i386-qemu, x86_64-efi, i386-xen,
                             x86_64-xen, mipsel-yeeloong-flash,
                             mipsel-fuloong2f-flash, mipsel-loongson-elf,
                             powerpc-ieee1275, sparc64-ieee1275-raw,
                             sparc64-ieee1275-cdcore, sparc64-ieee1275-aout,
                             ia64-efi, mips-arc, mipsel-arc,
                             mipsel-qemu_mips-elf, mips-qemu_mips-flash,
                             mipsel-qemu_mips-flash, mips-qemu_mips-elf,
                             arm-uboot, arm-efi, arm64-efi
  -p, --prefix=DIR           set prefix directory [default=/boot/grub]
  -v, --verbose              print verbose messages.
  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Report bugs to <bug-grub@gnu.org>.

~~~
