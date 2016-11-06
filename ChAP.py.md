# ChAP.py command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

RFIDIOtconfig module ERROR: option --help not recognized

RFIDIOt Options:

	-d		Debug on
	-f <num>	Use LibNFC device number <num> (implies -R READER_LIBNFC)
	-g		No GUI
	-h		Print detailed help message
	-n		No Init - do not initialise hardware
	-N		List available LibNFC devices
	-r <num>	Use PCSC device number <num> (implies -R READER_PCSC)
	-R <type>	Reader/writer type:
				READER_ACG:	ACG Serial
				READER_ACS:	PC/SC Subtype ACS
				READER_ANDROID:	Android
				READER_DEMOTAG:	DemoTag
				READER_FROSCH:	Frosch Hitag
				READER_LIBNFC:	libnfc
				READER_NONE:	None
				READER_OMNIKEY:	PC/SC Subtype OmniKey
				READER_PCSC:	PC/SC
				READER_SCM:	PC/SC Subtype SCM
	-l <line>	Line to use for reader/writer
	-L		List available PCSC devices
	-s <baud>	Speed of reader/writer
	-t <seconds>	Timeout for inactivity of reader/writer


ChAP.py - Chip And PIN in Python
Ver 0.1c

usage:

 ChAP.py [options] [PIN]

If the optional numeric PIN argument is given, the PIN will be verified (note that this
updates the PIN Try Counter and may result in the card being PIN blocked).

Options:

	-a		Bruteforce AIDs
	-A		Print list of known AIDs
	-d		Debug - Show PC/SC APDU data
	-e		Bruteforce EMV AIDs
	-f		Bruteforce files
	-h		Print detailed help message
	-o		Output to files ([AID]-FILExxRECORDxx.HEX)
	-p		Bruteforce primitives
	-r		Raw output - do not interpret EMV data
	-t		Use T1 protocol (default is T0)
	-v		Verbose on


~~~
