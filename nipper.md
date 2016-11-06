# nipper command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


[34m                     _                           ____
               _ __ (_)_ __  _ __   ___ _ __    / ->/|
              | '_ \| | '_ \| '_ \ / _ \ '__|  /<-_/ |
              | | | | | |_) | |_) |  __/ |     |   | /
              |_| |_|_| .__/| .__/ \___|_|     |___|/
                      |_|   |_|

                           Version 0.11.10
                     http://nipper.titania.co.uk
             Copyright (C) 2006-2008 Ian Ventura-Whiting

[0mNipper is a  Network Infrastructure  Configuration Parser.  Nipper takes
a network infrastructure  device configuration,  processes the  file and
details security-related  issues with detailed  recommendations.  Nipper
was previous known as CiscoParse.

By default, input is retrieved from stdin and is output (in HTML format)
to stdout.

[34mCommand:[0m
    [32mnipper [Options][0m

[34mGeneral Options:[0m
    [32m--input=<file>[0m
    Specifies a  device configuration  file to  process.  For CheckPoint
    Firewall-1 configurations, the input should be the conf directory.

    [32m--output=<file> | --report=<file>[0m
    Specified an output file for the report.

    [32m--csv=<file>[0m
    Want to output the network filtering configuration to a CSV file?.

    [32m--version[0m
    Displays the program version.

[34mExample:[0m
    The  example   below  will   process  a   Cisco   IOS-based   router
    configuration file called ios.conf  and output  the report to a file
    called report.html.

    [32mnipper --ios-router --input=ios.conf --output=report.html[0m

[34mFor additional help:[0m
    [32m--help[=<topic>][0m
    Show  the  online help  or show  the  additional  help on  the topic
    specified.  The help  topics  are;  GENERAL,  DEVICES,  DEVICES-ADV,
    SNMP,  REPORT, REPORT-ADV,  REPORT-SECT, REPORT-HTML,  REPORT-LATEX,
    AUDIT-ACL, AUDIT-PASS, AUDIT-ADV or CONFIG-FILE.

~~~
