# libnetcfg command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


/usr/bin/libnetcfg: Usage: /usr/bin/libnetcfg [-c] [-d] [-i oldconfigile] [-o newconfigfile] [-h]
Without options, the old configuration is shown.

   -c change the configuration
   -d use defaults from the old config (implies -c, non-interactive)
   -i use a specific file as the old config file
   -o use a specific file as the new config file
   -h show this help

The default name of the old configuration file is by default
"libnet.cfg", unless otherwise specified using the -i option,
C<-i oldfile>, and it is searched first from the current directory,
and then from your module path.

The default name of the new configuration file is "libnet.cfg", and by
default it is written to the current directory, unless otherwise
specified using the -o option.


~~~
