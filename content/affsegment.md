# affsegment command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

affsegment version 3.7.10
usage: affsegment [options] file1.aff [file2.aff ...]
options:
    -c              Create AFF files if they do not exist
    -ssegval        Sets the value of a segment; may be repeated
    -psegname       Prints the contents of the segment name for each file
    -V              Just print the version number and exit.
    -dname          Delete segment 'name'
    -h, -?          Print this message
    -Q              interpert 8-byte segments as a 64-bit value
    -A              Print the 32-bit arg, not the segment value
    -x              Print the segment as a hex string

Values for segval:

Setting the segment values:
    -sname=-        Take the new value of segment 'name' from stdin
    -sname=val      Sets segment 'name' to be 'val'  
    -sname=<val     Sets segment 'name' to be contents of file 'val'

Setting the segment args:
    -sname/arg       Sets segment 'name' arg to be 'arg'  (may be repeated)

Setting both the segment value and the arg:
    -sname/arg=val   Sets both arg and val for segment 'name'
    -sname/arg=<file Sets the arg and take contents from file 'file'
    -sname/arg=-     Sets the arg of segment 'name' and take the contents from stdin

Note: All deletions are done first, then all updates. Don't specify the
same segment twice on one command line.

~~~
