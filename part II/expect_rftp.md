# expect_rftp command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Once logged in, cd to the directory to be transferred and press:
~p to put the current directory from the local to the remote host
~g to get the current directory from the remote host to the local host
~l to list the current directory from the remote host
spawn ftp -h

	Usage: { ftp | pftp } [-46pinegvtd] [hostname]
	   -4: use IPv4 addresses only
	   -6: use IPv6, nothing else
	   -p: enable passive mode (default for pftp)
	   -i: turn off prompting during mget
	   -n: inhibit auto-login
	   -e: disable readline support, if present
	   -g: disable filename globbing
	   -v: verbose mode
	   -t: enable packet tracing [nonfunctional]
	   -d: enable debugging


~~~
