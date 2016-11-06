# rtpbreak command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Copyright (c) 2007-2008 Dallachiesa Michele <micheleDOTdallachiesaATposteDOTit>
rtpbreak v1.3a is free software, covered by the GNU General Public License.

USAGE: rtpbreak (-r|-i) <source> [options]

 INPUT

  -r <str>      Read packets from pcap file <str>
  -i <str>      Read packets from network interface <str>
  -L <int>      Force datalink header length == <int> bytes

 OUTPUT

  -d <str>      Set output directory to <str> (def:.)
  -w            Disable RTP raw dumps
  -W            Disable RTP pcap dumps
  -g            Fill gaps in RTP raw dumps (caused by lost packets)
  -n            Dump noise packets
  -f            Disable stdout logging
  -F            Enable syslog logging
  -v            Be verbose

 SELECT

  -m            Sniff packets in promisc mode
  -p <str>      Add pcap filter <str>
  -e            Expect even destination UDP port
  -u            Expect unprivileged source/destination UDP ports (>1024)
  -y <int>      Expect RTP payload type == <int>
  -l <int>      Expect RTP payload length == <int> bytes
  -t <float>    Set packet timeout to <float> seconds (def:10.00)
  -T <float>    Set pattern timeout to <float> seconds (def:0.25)
  -P <int>      Set pattern packets count to <int> (def:5)

 EXECUTION

  -Z <str>      Run as user <str>
  -D            Run in background (option -f implicit)

 MISC

  -k            List known RTP payload types
  -h            This


~~~
