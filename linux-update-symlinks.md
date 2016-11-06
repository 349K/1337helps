# linux-update-symlinks command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: /usr/bin/linux-update-symlinks {install|upgrade|remove} VERSION IMAGE-PATH

This command is intended to be called from the postinst and postrm
maintainer scripts of Linux kernel packages.  The postinst script must
pass the first argument 'install' or 'upgrade' depending on whether a
fresh installation or an upgrade has taken place.

The VERSION argument must be the kernel version string as shown by
'uname -r' and used in filenames.

The IMAGE-PATH argument must be the absolute filename of the kernel
image.

~~~
