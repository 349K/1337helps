# sorter command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Missing image argument

sorter [-b size] [-E] [-e] [-h]  [-l] [-md5] [-s] [-sha1] [-U] [-v] [-V] [-a hash_alert] [-c config] [-C config] [-d dir] [-m mnt] [-n nsrl_db] [-x hash_exclude] [-o imgoffset] [-f fstype] [-i imgtype] image [images] [dir_meta_addr] 

    -b size: Minimum size.  Ignore files smaller than 'size'
	-E: Perform category indexing only (no extension checks - was '-i')
	-e: Perform extension checks only (no category index files)
	-h: HTML Format
	-l: List index to STDOUT (no files are ever written)
	-md5: Print the MD5 value with the index output
	-s: Save files to category directories
	-sha1: Print the SHA-1 value with the index output
	-U: Ignore the unknown category - only save catgories in config files
	-v: verbose debugging output
	-V: print version information
	-a hash_alert: hash database of hashes to alert on
	-c config: specify a config file to use (in addition to default files)
	   NOTE: This config file has priority over default files
	-C config: specify the ONLY config file to use
	-d dir: Save category index files in the specified directory
	-f fstype: file system type (Sleuth Kit types) of image
	-i imgtype: Format of image file
	-o imgoffset: Offset of file system in image (in sectors)
	-m mnt: The mounting point of the image
	-n nsrl_db: The NIST NSRL database file (NSRLFile.txt) (hashes to ignore)
	-x hash_exclude: hash database of hashes to ignore
	dir_meta_addr: Address of directory to start analyzing from 
	image: image to analyze

~~~
