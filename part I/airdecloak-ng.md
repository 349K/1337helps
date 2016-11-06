# airdecloak-ng command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


  Airdecloak-ng 1.2 rc4 - (C) 2008-2015 Thomas d'Otreppe
  http://www.aircrack-ng.org

  usage: airdecloak-ng [options]

  options:

   Mandatory:
     -i <file>             : Input capture file
     --ssid <ESSID>        : ESSID of the network to filter
        or
     --bssid <BSSID>       : BSSID of the network to filter

   Optional:
     -o <file>             : Output packets (valid) file (default: <src>-filtered.pcap)
     -c <file>             : Output packets (cloaked) file (default: <src>-cloaked.pcap)
     -u <file>             : Output packets (unknown/ignored) file (default: invalid_status.pcap)
     --filters <filters>   : Apply filters (separated by a comma). Filters:
           signal:               Try to filter based on signal.
           duplicate_sn:         Remove all duplicate sequence numbers
                                 for both the AP and the client.
           duplicate_sn_ap:      Remove duplicate sequence number for
                                 the AP only.
           duplicate_sn_client:  Remove duplicate sequence number for the
                                 client only.
           consecutive_sn:       Filter based on the fact that IV should
                                 be consecutive (only for AP).
           duplicate_iv:         Remove all duplicate IV.
           signal_dup_consec_sn: Use signal (if available), duplicate and
                                 consecutive sequence number (filtering is
                                  much more precise than using all these
                                  filters one by one).
     --null-packets        : Assume that null packets can be cloaked.
     --disable-base_filter : Do not apply base filter.
     --drop-frag           : Drop fragmented packets

     --help                : Displays this usage screen


~~~
