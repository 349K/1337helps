# affcat command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

affcat version 3.7.10
usage: affcat [options] infile [... more infiles]
options:
    -s name --- Just output segment name
    -p ###  --- just output data page number ###
    -S ###  --- Just output data sector ### (assumes 512-byte sectors). Sector #0 is first
    -q      --- quiet; don't print to STDERR if a page is skipped
    -n      --- noisy; tell when pages are skipped.
    -l      --- List all of the segment names
    -L      --- List segment names, lengths, and args
    -d      --- debug. Print the page numbers to stderr as data goes to stdout
    -b      --- Output BADFALG for bad blocks (default is NULLs)
    -v      --- Just print the version number and exit.
    -r offset:count --- seek to offset and output count characters in each file; may be repeated

~~~
