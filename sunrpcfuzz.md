# sunrpcfuzz command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
sunrpcfuzz -h <target host> <-s and/or -a> [optional args]
	-s <n>	Test a specific RCP program 'n' [requires -v, and -p]
	-a	Test all registered RPC programs

WARNING: avoid running with -a or -s 100000 against
localhost--doing so will probably register a bunch of bogus
RPC programs with the local portmapper.

Optional Arguments:
	-v <program version>
	-p <protocol number, 17 for UDP or 6 for TCP>
	-i <n>	Do 'n' fuzzed messages per procedure
	-l <n>	'n' is last procedure to test
	-f <n>	'n' is first procedure to test
	-r <n>	Push 'n' random xdr items onto the SPIKE


~~~
