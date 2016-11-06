# gbb_utility command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:  futility gbb_utility [-g|-s|-c] [OPTIONS] bios_file [output_file]

GET MODE:
-g, --get   (default)	Get (read) from bios_file, with following options:
     --hwid          	Report hardware id (default).
     --flags         	Report header flags.
     --digest        	Report digest of hwid (>= v1.2)
     --roothash      	Check ryu root key hash
 -k, --rootkey=FILE  	File name to export Root Key.
 -b, --bmpfv=FILE    	File name to export Bitmap FV.
 -r  --recoverykey=FILE	File name to export Recovery Key.

SET MODE:
-s, --set            	Set (write) to bios_file, with following options:
 -o, --output=FILE   	New file name for ouptput.
     --hwid=HWID     	The new hardware id to be changed.
     --flags=FLAGS   	The new (numeric) flags value.
 -k, --rootkey=FILE  	File name of new Root Key.
 -b, --bmpfv=FILE    	File name of new Bitmap FV.
 -r  --recoverykey=FILE	File name of new Recovery Key.

CREATE MODE:
-c, --create=hwid_size,rootkey_size,bmpfv_size,recoverykey_size
                     	Create a GBB blob by given size list.
SAMPLE:
  gbb_utility -g bios.bin
  gbb_utility --set --hwid='New Model' -k key.bin bios.bin newbios.bin
  gbb_utility -c 0x100,0x1000,0x03DE80,0x1000 gbb.blob


~~~
