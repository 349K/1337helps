# cisco-torch command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Using config file torch.conf...
Loading include and plugin ...
 version 
usage: cisco-torch <options> <IP,hostname,network>

or: cisco-torch <options> -F <hostlist>

Available options:
-O <output file>
-A		All fingerprint scan types combined
-t		Cisco Telnetd scan
-s		Cisco SSHd scan
-u		Cisco SNMP scan
-g		Cisco config or tftp file download
-n		NTP fingerprinting scan
-j		TFTP fingerprinting scan
-l <type>	loglevel
		c  critical (default)
		v  verbose
		d  debug
-w		Cisco Webserver scan
-z		Cisco IOS HTTP Authorization Vulnerability Scan
-c		Cisco Webserver with SSL support scan
-b		Password dictionary attack (use with -s, -u, -c, -w , -j or -t only)
-V		Print tool version and exit
examples:	cisco-torch -A 10.10.0.0/16
		cisco-torch -s -b -F sshtocheck.txt
		cisco-torch -w -z 10.10.0.0/16
		cisco-torch -j -b -g -F tftptocheck.txt

~~~
