# usbhid-dump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: usbhid-dump [OPTION]...
Dump USB device HID report descriptor(s) and/or stream(s).

Options:
  -h, --help                       output this help message and exit
  -v, --version                    output version information and exit

  -s, -a, --address=bus[:dev]      limit interfaces by bus number
                                   (1-255) and device address (1-255),
                                   decimal; zeroes match any
  -d, -m, --model=vid[:pid]        limit interfaces by vendor and
                                   product IDs (0001-ffff), hexadecimal;
                                   zeroes match any
  -i, --interface=NUMBER           limit interfaces by number (0-254),
                                   decimal; 255 matches any

  -e, --entity=STRING              what to dump: either "descriptor",
                                   "stream" or "all"; value can be
                                   abbreviated

  -t, --stream-timeout=NUMBER      stream interrupt transfer timeout, ms;
                                   zero means infinity
  -p, --stream-paused              start with the stream dump output
                                   paused
  -f, --stream-feedback            enable stream dumping feedback: for
                                   every transfer dumped a dot is
                                   printed to stderr

Default options: --stream-timeout=60000 --entity=descriptor

Signals:
  USR1/USR2                        pause/resume the stream dump output


~~~
