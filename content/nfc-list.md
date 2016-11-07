# nfc-list command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

nfc-list uses libnfc 1.7.1
usage: nfc-list [-v] [-t X]
  -v	 verbose display
  -t X	 poll only for types according to bitfield X:
	   1: ISO14443A
	   2: Felica (212 kbps)
	   4: Felica (424 kbps)
	   8: ISO14443B
	  16: ISO14443B'
	  32: ISO14443B-2 ST SRx
	  64: ISO14443B-2 ASK CTx
	 128: Jewel
	So 255 (default) polls for all types.
	Note that if 16, 32 or 64 then 8 is selected too.

~~~
