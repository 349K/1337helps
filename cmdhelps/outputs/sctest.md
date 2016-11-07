# sctest command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


	-a PATH    		use this argos csi files as input
	--argos-csi=   PATH 

	-b IP:PORT 		bind this ip:port
	--bind=IP:PORT 

	-c IP:PORT 		redirect connects to this ip:port
	--connect=IP:PORT 

	-C CMD     		command to execute for "cmd" in shellcode (default: cmd="/bin/sh -c \"cd ~/.wine/drive_c/; wine 'c:\windows\system32\cmd_orig.exe' \"")
	--cmd=    CMD 

	-d INTEGER 		dump the shellcode (binary) to stdout
	--dump=INTEGER 

	-g         		run getpc mode, try to detect a shellcode
	--getpc

	-G FILEPATH 		save a dot formatted callgraph in filepath
	--graph=FILEPATH 

	-h         		show this help
	--help

	-i         		proxy api calls to the host operating system
	--interactive

	-l         		list all tests
	--listtests

	-o [INT|HEX] 		manual offset for shellcode, accepts int and hexvalues
	--offset=[INT|HEX] 

	-p PATH    		write shellcode profile to this file
	--profile=   PATH 

	-S         		read shellcode/buffer from stdin, works with -g
	--stdin

	-s INTEGER 		max number of steps to run
	--steps=INTEGER 

	-t INTEGER 		the test to run
	--testnumber=INTEGER 

	-v         		be verbose, can be used multiple times, f.e. -vv
	--verbose


~~~
