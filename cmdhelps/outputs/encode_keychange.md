# encode_keychange command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: encode_keychange [-fhPvV] -t (md5|sha1) [-O "<old_passphrase>"][-N "<new_passphrase>"][-E [0x]<engineID>]

    -E [0x]<engineID>		EngineID used for kul generation.
    -f				Force passphrases to be read from stdin.
    -h				Help.
    -N "<new_passphrase>"	Passphrase used to generate new Ku.
    -O "<old_passphrase>"	Passphrase used to generate old Ku.
    -P				Turn off prompt indicators.
    -t md5 | sha1		HMAC hash transform type.
    -v				Verbose.
    -V				Visible.  Echo passphrases to terminal.
		

Only -t is mandatory.  The transform is used to convert P=>Ku, convert
    Ku=>Kul, and to hash the old Kul with the random bits.

    Passphrase will be taken from the first successful source as follows:
	a) Commandline options,
	b) The file "/root/.snmp/passphrase.ek",
	c) stdin  -or-  User input from the terminal.

-f will require reading from the stdin/terminal, ignoring a) and b).
    -P will prevent prompts for passphrases to stdout from being printed.

    <engineID> is interpreted as a hex string when preceded by "0x",
    otherwise it is created to contain "text".  If nothing is given,
    <engineID> is constructed from the first IP address for the local host.
		

~~~
