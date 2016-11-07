# gpg-agent command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


gpg-agent (GnuPG) 2.1.11
libgcrypt 1.7.3-beta
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Syntax: gpg-agent [options] [command [args]]
Secret key management for GnuPG

Options:
 
     --daemon                     run in daemon mode (background)
     --server                     run in server mode (foreground)
 -v, --verbose                    verbose
 -q, --quiet                      be somewhat more quiet
 -s, --sh                         sh-style command output
 -c, --csh                        csh-style command output
     --options FILE               read options from FILE
     --no-detach                  do not detach from the console
     --no-grab                    do not grab keyboard and mouse
     --log-file                   use a log file for the server
     --pinentry-program PGM       use PGM as the PIN-Entry program
     --scdaemon-program PGM       use PGM as the SCdaemon program
     --disable-scdaemon           do not use the SCdaemon
     --extra-socket NAME          accept some commands via NAME
     --keep-tty                   ignore requests to change the TTY
     --keep-display               ignore requests to change the X display
     --default-cache-ttl N        expire cached PINs after N seconds
     --ignore-cache-for-signing   do not use the PIN cache when signing
     --no-allow-external-cache    disallow the use of an external password cache
     --no-allow-mark-trusted      disallow clients to mark keys as "trusted"
     --allow-preset-passphrase    allow presetting passphrase
     --allow-loopback-pinentry    allow caller to override the pinentry
     --allow-emacs-pinentry       allow passphrase to be prompted through Emacs
     --enable-ssh-support         enable ssh support

Please report bugs to <http://bugs.gnupg.org>.

~~~
