# fiwalk command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: fiwalk [options] iso-name
Default behavior: Just print the file system statistics and exit.
options:
    -c config.txt   read config.txt for metadata extraction tools
    -C nn           only process nn files, then do a clean exit

include/exclude parameters; may be repeated. 
    -n pattern  = only match files for which the filename matches
                  the pattern.
              example: -n .jpeg -n .jpg will find all JPEG files
              Case is ignored. Will not match orphan files.
    
Ways to make this program run faster:
    -I ignore NTFS system files
    -g just report the file objects - don't get the data
    -O only walk allocated files
    -b do not report byte runs if data not accessed
    -z do not calculate MD5 or SHA1 values
    -Gnn - Only process the contents of files smaller than nn gigabytes (default 2)
           (Specify -G0 to remove space restrictions)

Ways to make this program run slower:
    -M = Report MD5 for each file (default on)
    -1 = Report SHA1 for each file (default on)
    -S nnnn = Perform sector hashes every nnnn bytes
    -f = Report the output of the 'file' command for each

Output options:
    -m = Output in SleuthKit 'Body file' format
    -A<file> = ARFF output to <file>
    -X<file> = XML output to a <file> (full DTD)
         -X0 = Write output to filename.xml
    -Z       = zap (erase) the output file
    -x       = XML output to stdout (no DTD)
    -T<file> = Walkfile output to <file>
    -a <audit.txt> = Read the scalpel audit.txt file

Misc:
    -d = debug this program
    -v = Enable SleuthKit verbose flag

SleuthKit Version: 4.2.0
AFFLIB Version:    3.7.10
LIBEWF Version:    20140608

~~~
