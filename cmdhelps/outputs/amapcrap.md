# amapcrap command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


amapcrap v5.4 (c) 2011 by van Hauser/THC <vh@thc.org>

Syntax: amapcrap [-S] [-u] [-m 0ab] [-M min,max] [-n connects] [-N delay] [-w delay] [-e] [-v] TARGET PORT

Options:
    -S           use SSL after TCP connect (not usuable with -u)
    -u           use UDP protocol (default: TCP) (not usable with -c)
    -n connects  maximum number of connects (default: unlimited)
    -N delay     delay between connects in ms (default: 0)
    -w delay     delay before closing the port (default: 250)
    -e           do NOT stop when a response was made by the server
    -v           verbose mode
    -m 0ab       send as random crap:0-nullbytes, a-letters+spaces, b-binary
    -M min,max   minimum and maximum length of random crap
    TARGET PORT  target (ip or dns) and port to send random crap

This tool sends random data to a silent port to illicit a response, which can
then be used within amap for future detection. It outputs proper amap
appdefs definitions. Note: by default all modes are activated (0:10%, a:40%,
b:50%). Mode 'a' always sends one line with letters and spaces which end with
\r\n. Visit our homepage at http://www.thc.org

~~~
