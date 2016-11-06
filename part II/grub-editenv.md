# grub-editenv command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: grub-editenv [OPTION...] FILENAME COMMAND

Tool to edit environment block.

 Commands:
  create                     Create a blank environment block file.
  list                       List the current variables.
  set [NAME=VALUE ...]       Set variables.
  unset [NAME ...]           Delete variables.

  -?, --help                 give this help list
      --usage                give a short usage message
  -v, --verbose              print verbose messages.
  -V, --version              print program version

 Options:

If FILENAME is `-', the default value /boot/grub/grubenv is used.

There is no `delete' command; if you want to delete the whole environment
block, use `rm /boot/grub/grubenv'.

Report bugs to <bug-grub@gnu.org>.

~~~
