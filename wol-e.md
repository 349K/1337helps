# wol-e command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



[*] WOL-E 1.0
[*] Wake on LAN Explorer - A collection a WOL tools.
[*] by Nathaniel Carew

	-m
		Waking up single computers.
		If a password is required use the -k 00:12:34:56:78:90 at the end of the above command.
		wol-e -m 00:12:34:56:78:90 -b 192.168.1.255 -p <port> -k <pass>
		Defaults: 
		Port: 9
		Broadcast: 255.255.255.255
		Pass: empty

	-s
		Sniffing the network for WOL requests and passwords.
		All captured WOL requests will be displayed on screen and written to /usr/share/wol-e/WOLClients.txt.
		wol-e -s -i eth0

	-a
		Bruteforce powering on WOL clients.
		wol-e -a -p <port>
		Place the address ranges into the bfmac.lst that you wish to bruteforce.
		They should be in the following format:
		00:12:34:56
		Default port: 9

	-f
		Detecting Apple devices on the network for WOL enabling.
		This will output to the screen and write to /usr/share/wol-e/AppleTargets.txt for detected Apple MAC's.
		wol-e -f

	-fa
		Attempt to wake all detected Apple targets in /usr/share/wol-e/AppleTargets.txt.
		This will send a single WOL packet to each client in the list and tell you how many clients were attempted.
		wol-e -fa


~~~
