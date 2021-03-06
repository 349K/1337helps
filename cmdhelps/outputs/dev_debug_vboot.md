# dev_debug_vboot command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: dev_debug_vboot [options] [DIRECTORY]

This logs as much as it can about the verified boot process. With no arguments
it will attempt to read the current BIOS, extract the firmware keys, and use
those keys to validate all the ChromeOS kernel partitions it can find. A
summary output is printed on stdout, and the detailed log is copied to
/var/log/debug_vboot_noisy.log afterwards.

If a directory is given, it will attempt to use the components from that
directory and will leave the detailed log in that directory.

Options:

   -b FILE, --bios FILE        Specify the BIOS image to use
   -i FILE, --image FILE       Specify the disk image to use
   -k FILE, --kernel FILE      Specify the kernel partition image to use
   -v                          Spew the detailed log to stdout

   -c, --cleanup               Delete the DIRECTORY when done

   -h, --help                  Print this help message and exit


~~~
