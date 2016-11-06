# svreport command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: svreport [command] [options]

Supported commands:

                - list:	lists all scans

                - export:	exports the given scan to a given format

                - delete:	deletes the scan

                - stats:	print out some statistics of interest

                - search:	search for a specific string in the user agent (svmap)

examples:

      svreport.py list

      svreport.py export -f pdf -o scan1.pdf -s scan1

      svreport.py delete -s scan1



Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -v, --verbose         Increase verbosity
  -q, --quiet           Quiet mode
  -t SESSIONTYPE, --type=SESSIONTYPE
                        Type of session. This is usually either svmap, svwar
                        or svcrack. If not set I will try to find the best
                        match
  -s SESSION, --session=SESSION
                        Name of the session
  -f FORMAT, --format=FORMAT
                        Format type. Can be stdout, pdf, xml, csv or txt
  -o OUTPUTFILE, --output=OUTPUTFILE
                        Output filename
  -n                    Do not resolve the ip address
  -c, --count           Used togather with 'list' command to count the number
                        of entries

~~~
