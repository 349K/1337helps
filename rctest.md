# rctest command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

rctest - RFCOMM testing
Usage:
	rctest <mode> [options] [bdaddr]
Modes:
	-r listen and receive
	-w listen and send
	-d listen and dump incoming data
	-s connect and send
	-u connect and receive
	-n connect and be silent
	-c connect, disconnect, connect, ...
	-m multiple connects
	-a automated test (receive hcix as parameter)
Options:
	[-b bytes] [-i device] [-P channel] [-U uuid]
	[-L seconds] enabled SO_LINGER option
	[-W seconds] enable deferred setup
	[-B filename] use data packets from file
	[-O filename] save received data to file
	[-N num] number of frames to send
	[-C num] send num frames before delay (default = 1)
	[-D milliseconds] delay after sending num frames (default = 0)
	[-Y priority] socket priority
	[-A] request authentication
	[-E] request encryption
	[-S] secure connection
	[-M] become master
	[-T] enable timestamps

~~~
