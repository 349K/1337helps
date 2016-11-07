# webacoo command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



	WeBaCoo 0.2.3 - Web Backdoor Cookie Script-Kit
	Copyright (C) 2011-2012 Anestis Bechtsoudis
	{ @anestisb | anestis@bechtsoudis.com | http(s)://bechtsoudis.com }


Usage: webacoo.pl [options]

Options:
  -g		Generate backdoor code (-o is required)

  -f FUNCTION	PHP System function to use
	FUNCTION
		1: system 	(default)
		2: shell_exec
		3: exec
		4: passthru
		5: popen

  -o OUTPUT	Generated backdoor output filename

  -r 		Return un-obfuscated backdoor code

  -t		Establish remote "terminal" connection (-u is required)

  -u URL	Backdoor URL

  -e CMD	Single command execution mode (-t and -u are required)

  -m METHOD	HTTP method to be used (default is GET)

  -c C_NAME	Cookie name (default: "M-cookie")

  -d DELIM	Delimiter (default: New random for each request)

  -a AGENT	HTTP header user-agent (default exist)

  -p PROXY	Use proxy (tor, ip:port or user:pass:ip:port)

  -v LEVEL	Verbose level
	LEVEL
		0: no additional info (default)
		1: print HTTP headers
		2: print HTTP headers + data

  -l LOG	Log activity to file

  -h		Display help and exit

  update	Check for updates and apply if any

~~~
