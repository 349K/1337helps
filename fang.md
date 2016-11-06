# fang command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

redfang - the bluetooth hunter ver 2.5
(c)2003 @stake Inc
author:   Ollie Whitehouse <ollie@atstake.com>
enhanced: threads by Simon Halsall <s.halsall@eris.qinetiq.com>
enhanced: device info discovery by Stephen Kapp <skapp@atstake.com>
usage:
   fang [options]

options:
   -r	range      i.e. 00803789EE76-00803789EEff
   -o	filename   Output Scan to Text Logfile
     	           An address can also be manf+nnnnnn, where manf
     	           is listed with the -l option and nnnnnn is the
     	           tail of the address. All addresses must be 12
     	           characters long
   -t	timeout    The connect timeout, this is 10000 by default
     	           Which is quick and yields results, increase for
     	           reliability
   -n	num        The number of dongles
   -d	           Show debug information
   -s	           Perform Bluetooth Discovery
   -l	           Show device manufacturer codes

   -h              Display help

The devices are assumed to be hci0 to hci(n) where (n) is the number
of threads -1, this is currently not configurable but maybe at a
later date

~~~
