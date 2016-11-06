# knocker command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

knocker, the net portscanner. Version 0.7.1 (24 May 2002)

Usage: knocker --host <HOST> [OPTIONS]

Example: knocker -H 192.168.0.1 -SP 1 -EP 1024

Required options:
      -H,  --host              host name or numeric Internet address
        or
      --last-host              get the last scanned host name

Common options (if SP is specified you must also give EP):
      -P,  --port              single port number (for one port scans only)
      -SP, --start-port        port number to begin the scan from
      -EP, --end-port          port number to end the scan at

      --last-scan              performs again the last port scan

Extra options:
      -4,  --ipv4              only IPv4 host addressing
      -6,  --ipv6              only IPv6 host addressing
      -q,  --quiet             quiet mode (no console output, logs to file)
      -lf, --logfile <logfile> log scan results to the specified file
      -nf, --no-fency          disable fancy output
      -nc, --no-colors         disable colored output

      --configure              let you configure knocker

Info options:
      -h,  --help              display this help and exit
      -v,  --version           output version information and exit

SEE THE MAN PAGE FOR MORE DESCRIPTIONS, AND EXAMPLES
Report bugs to <g.gabriele79@genie.it>.

~~~
