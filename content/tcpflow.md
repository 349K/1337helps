# tcpflow command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

TCPFLOW version 1.4.5

usage: tcpflow [-aBcCDhJpsvVZ] [-b max_bytes] [-d debug_level] 
     [-[eE] scanner] [-f max_fds] [-F[ctTXMkmg]] [-i iface] [-L semlock]
     [-m min_bytes] [-o outdir] [-r file] [-R file] 
     [-S name=value] [-T template] [-w file] [-x scanner] [-X xmlfile]
      [expression]

   -a: do ALL post-processing.
   -b max_bytes: max number of bytes per flow to save
   -d debug_level: debug level; default is 1
   -f: maximum number of file descriptors to use
   -h: print this help message (-hh for more help)
   -H: print detailed information about each scanner
   -i: network interface on which to listen
   -I: generate temporal packet-> byte index files for each flow (.findex)
   -g: output each flow in alternating colors (note change!)
   -l: treat non-flag arguments as input files rather than a pcap expression
   -L  semlock - specifies that writes are locked using a named semaphore
   -p: don't use promiscuous mode
   -q: quiet mode - do not print warnings
   -r file: read packets from tcpdump pcap file (may be repeated)
   -R file: read packets from tcpdump pcap file TO FINISH CONNECTIONS
   -v: verbose operation equivalent to -d 10
   -V: print version number and exit
   -w file: write packets not processed to file
   -o  outdir   : specify output directory (default '.')
   -X  filename : DFXML output to filename
   -m  bytes    : specifies skip that starts a new stream (default 16777216).
   -F{p} : filename prefix/suffix (-hh for options)
   -T{t} : filename template (-hh for options; default %A.%a-%B.%b%V%v%C%c)
   -Z: do not decompress gzip-compressed HTTP transactions

Control of Scanners:
   -E scanner   - turn off all scanners except scanner
   -S name=value  Set a configuration parameter (-hh for info)

Settable Options (and their defaults): 
   -S enable_report=YES    Enable report.xml ()
   -S http_cmd=    Command to execute on each HTTP attachment (http)
   -S http_alert_fd=-1    File descriptor to send information about completed HTTP attachments (http)
   -S netviz_histogram_dump=0    Dumps the histogram (netviz)
   -S netviz_histogram_size=1000    Maximum histogram size (netviz)
   -S tcp_timeout=0    Timeout for TCP connections (tcpdemux)
   -S check_fcs=YES    Require valid Frame Check Sum (FCS) (wifiviz)

   -e http - enable scanner http
   -e md5 - enable scanner md5
   -e netviz - enable scanner netviz
   -e wifiviz - enable scanner wifiviz

   -x tcpdemux - disable scanner tcpdemux
Console output options:
   -B: binary output, even with -c or -C (normally -c or -C turn it off)
   -c: console print only (don't create files)
   -C: console print only, but without the display of source/dest header
   -0: don't print newlines after packets when printing to console   -s: strip non-printable characters (change to '.')
   -D: output in hex (useful to combine with -c or -C)

expression: tcpdump-like filtering expression

See the man page for additional information.

Filename Prefixes:
   -Fc : append the connection counter to ALL filenames
   -Ft : prepend the time_t timestamp to ALL filenames
   -FT : prepend the ISO8601 timestamp to ALL filenames
   -FX : Do not output any files (other than report files)
   -FM : Calculate the MD5 for every flow (stores in DFXML)
   -Fk : Bin output in 1K directories
   -Fm : Bin output in 1M directories (2 levels)
   -Fg : Bin output in 1G directories (3 levels)
Filename template format:
  %A/%a - source IP address/port;          %B/%b - dest IP address/port
  %E/%e - source/dest Ethernet Mac address
  %V/%v - VLAN number, '--' if no vlan/'' if no vlan
  %T/%t - Timestamp in ISO8601 format/unix time_t
  %c - connection_count for connections>0 / %# for all connections;  %C - 'c' if connection_count >0
  %N - (connection_number )             % 1000
  %K - (connection_number / 1000)       % 1000
  %M - (connection_number / 1000000)    % 1000
  %G - (connection_number / 1000000000) % 1000
  %% - Output a '%'

-S name=value options:
   tdelta=0             Time delta in seconds

DEBUG Levels (specify with -dNN):
get_max_fds() = 1024
NUM_RESERVED_FDS = 6

~~~
