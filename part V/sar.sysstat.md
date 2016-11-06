# sar.sysstat command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: sar.sysstat [ options ] [ <interval> [ <count> ] ]
Main options and reports:
	-B	Paging statistics
	-b	I/O and transfer rate statistics
	-d	Block devices statistics
	-F [ MOUNT ]
		Filesystems statistics
	-H	Hugepages utilization statistics
	-I { <int> | SUM | ALL | XALL }
		Interrupts statistics
	-m { <keyword> [,...] | ALL }
		Power management statistics
		Keywords are:
		CPU	CPU instantaneous clock frequency
		FAN	Fans speed
		FREQ	CPU average clock frequency
		IN	Voltage inputs
		TEMP	Devices temperature
		USB	USB devices plugged into the system
	-n { <keyword> [,...] | ALL }
		Network statistics
		Keywords are:
		DEV	Network interfaces
		EDEV	Network interfaces (errors)
		NFS	NFS client
		NFSD	NFS server
		SOCK	Sockets	(v4)
		IP	IP traffic	(v4)
		EIP	IP traffic	(v4) (errors)
		ICMP	ICMP traffic	(v4)
		EICMP	ICMP traffic	(v4) (errors)
		TCP	TCP traffic	(v4)
		ETCP	TCP traffic	(v4) (errors)
		UDP	UDP traffic	(v4)
		SOCK6	Sockets	(v6)
		IP6	IP traffic	(v6)
		EIP6	IP traffic	(v6) (errors)
		ICMP6	ICMP traffic	(v6)
		EICMP6	ICMP traffic	(v6) (errors)
		UDP6	UDP traffic	(v6)
		FC	Fibre channel HBAs
	-q	Queue length and load average statistics
	-R	Memory statistics
	-r [ ALL ]
		Memory utilization statistics
	-S	Swap space utilization statistics
	-u [ ALL ]
		CPU utilization statistics
	-v	Kernel tables statistics
	-W	Swapping statistics
	-w	Task creation and system switching statistics
	-y	TTY devices statistics

~~~
