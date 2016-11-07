# savelog command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: savelog [-m mode] [-u user] [-g group] [-t] [-c cycle] [-p]
             [-j] [-C] [-d] [-l] [-r rolldir] [-n] [-q] file ...
	-m mode	   - chmod log files to mode
	-u user	   - chown log files to user
	-g group   - chgrp log files to group
	-c cycle   - save cycle versions of the logfile (default: 7)
	-r rolldir - use rolldir instead of . to roll files
	-C	   - force cleanup of cycled logfiles
	-d	   - use standard date for rolling
	-D	   - override date format for -d
	-t	   - touch file
	-l	   - don't compress any log files (default: compress)
	-p         - preserve mode/user/group of original file
	-j         - use bzip2 instead of gzip
	-J         - use xz instead of gzip
	-1 .. -9   - compression strength or memory usage (default: 9, except for xz)
	-x script  - invoke script with rotated log file in $FILE
	-n         - do not rotate empty files
	-q         - suppress rotation message
	file 	   - log file names

~~~
