# rfcomm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

RFCOMM configuration utility ver 5.36
Usage:
	rfcomm [options] <command> <dev>

Options:
	-i, --device [hciX|bdaddr]     Local HCI device or BD Address
	-h, --help                     Display help
	-r, --raw                      Switch TTY into raw mode
	-A, --auth                     Enable authentication
	-E, --encrypt                  Enable encryption
	-S, --secure                   Secure connection
	-M, --master                   Become the master of a piconet
	-L, --linger [seconds]         Set linger timeout
	-a                             Show all devices (default)

Commands:
	bind     <dev> <bdaddr> [channel]	Bind device
	release  <dev>                   	Release device
	show     <dev>                   	Show device
	connect  <dev> <bdaddr> [channel]	Connect device
	listen   <dev> [channel [cmd]]   	Listen
	watch    <dev> [channel [cmd]]   	Watch


~~~
