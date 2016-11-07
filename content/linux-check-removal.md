# linux-check-removal command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: /usr/bin/linux-check-removal VERSION

This command is intended to be called from the prerm maintainer scripts
of Linux kernel packages.

The VERSION argument must be the kernel version string as shown by
'uname -r' and used in filenames.

If the currently running kernel matches VERSION, linux-check-removal
will normally prompt the user to confirm this potentially dangerous
action and will fail if the user chooses to abort.  However, if the
current environment is in a chroot or container, or if debconf
prompts are disabled, it will always succeed without prompting.

~~~
