# packetforge-ng command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


  Packetforge-ng 1.2 rc4 - (C) 2006-2015 Thomas d'Otreppe
  Original work: Martin Beck
  http://www.aircrack-ng.org

  Usage: packetforge-ng <mode> <options>

  Forge options:

      -p <fctrl>     : set frame control word (hex)
      -a <bssid>     : set Access Point MAC address
      -c <dmac>      : set Destination  MAC address
      -h <smac>      : set Source       MAC address
      -j             : set FromDS bit
      -o             : clear ToDS bit
      -e             : disables WEP encryption
      -k <ip[:port]> : set Destination IP [Port]
      -l <ip[:port]> : set Source      IP [Port]
      -t ttl         : set Time To Live
      -w <file>      : write packet to this pcap file
      -s <size>      : specify size of null packet
      -n <packets>   : set number of packets to generate

  Source options:

      -r <file>      : read packet from this raw file
      -y <file>      : read PRGA from this file

  Modes:

      --arp          : forge an ARP packet    (-0)
      --udp          : forge an UDP packet    (-1)
      --icmp         : forge an ICMP packet   (-2)
      --null         : build a null packet    (-3)
      --custom       : build a custom packet  (-9)

      --help         : Displays this usage screen


~~~
