# partx command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 partx [-a|-d|-s|-u] [--nr <n:m> | <partition>] <disk>

Tell the kernel about the presence and numbering of partitions.

Options:
 -a, --add            add specified partitions or all of them
 -d, --delete         delete specified partitions or all of them
 -u, --update         update specified partitions or all of them
 -s, --show           list partitions

 -b, --bytes          print SIZE in bytes rather than in human readable format
 -g, --noheadings     don't print headings for --show
 -n, --nr <n:m>       specify the range of partitions (e.g. --nr 2:4)
 -o, --output <list>  define which output columns to use
 -P, --pairs          use key="value" output format
 -r, --raw            use raw output format
 -t, --type <type>    specify the partition type (dos, bsd, solaris, etc.)
 -v, --verbose        verbose mode

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Available columns (for --show, --raw or --pairs):
         NR  partition number
      START  start of the partition in sectors
        END  end of the partition in sectors
    SECTORS  number of sectors
       SIZE  human readable size
       NAME  partition name
       UUID  partition UUID
       TYPE  partition type (a string, a UUID, or hex)
      FLAGS  partition flags
     SCHEME  partition table type (dos, gpt, ...)

For more details see partx(8).

~~~
