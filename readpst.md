# readpst command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

ReadPST / LibPST v0.6.59
Little Endian implementation being used.
Usage: readpst [OPTIONS] {PST FILENAME}
OPTIONS:
	-V	- Version. Display program version
	-C charset	- character set for items with an unspecified character set
	-D	- Include deleted items in output
	-M	- Write emails in the MH (rfc822) format
	-S	- Separate. Write emails in the separate format
	-b	- Don't save RTF-Body attachments
	-c[v|l]	- Set the Contact output mode. -cv = VCard, -cl = EMail list
	-d <filename> 	- Debug to file.
	-e	- As with -M, but include extensions on output files
	-h	- Help. This screen
	-j <integer>	- Number of parallel jobs to run
	-k	- KMail. Output in kmail format
	-m	- As with -e, but write .msg files also
	-o <dirname>	- Output directory to write files to. CWD is changed *after* opening pst file
	-q	- Quiet. Only print error messages
	-r	- Recursive. Output in a recursive format
	-t[eajc]	- Set the output type list. e = email, a = attachment, j = journal, c = contact
	-u	- Thunderbird mode. Write two extra .size and .type files
	-w	- Overwrite any output mbox files

Only one of -M -S -e -k -m -r should be specified

~~~
