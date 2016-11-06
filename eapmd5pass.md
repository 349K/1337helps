# eapmd5pass command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

eapmd5pass - Dictionary attack against EAP-MD5

Usage: eapmd5pass [ -i <int> | -r <pcapfile> ] [ -w wordfile ] [options]

  -i <iface>	interface name
  -r <pcapfile>	read from a named libpcap file
  -w <wordfile>	use wordfile for possible passwords.
  -b <bssid>	BSSID of target network (default: all)
  -U <username>	Username of EAP-MD5 user.
  -C <chal>	EAP-MD5 challenge value.
  -R <response>	EAP-MD5 response value.
  -E <eapid>	EAP-MD5 response EAP ID value.
  -v		increase verbosity level (max 3)
  -V		version information
  -h		usage information

The "-r" and "[-U|-C|-R|-E]" options are not meant to be used together.  Use -r
when a packet capture is available.  Specify the username, challenge and
response when available through other means.

~~~
