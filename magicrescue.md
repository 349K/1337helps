# magicrescue command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: magicrescue [-I FILE] [-M MODE] [-O [+-=][0x]OFFSET] [-b BLOCKSIZE]
	-d OUTPUT_DIR -r RECIPE1 [-r RECIPE2 [...]] DEVICE1 [DEVICE2 [...]]

  -b  Only consider files starting at a multiple of BLOCKSIZE.
  -d  Mandatory.  Output directory for found files.
  -r  Mandatory.  Recipe name, file or directory.
  -I  Read input file names from this file ("-" for stdin)
  -M  Produce machine-readable output to stdout.
  -O  Resume from specified offset (hex or decimal) in the first device.


~~~
