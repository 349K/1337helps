# maskgen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: maskgen pass0.masks [pass1.masks ...] [options]

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -t 86400, --targettime=86400
                        Target time of all masks (seconds)
  -o masks.hcmask, --outputmasks=masks.hcmask
                        Save masks to a file
  --showmasks           Show matching masks

  Individual Mask Filter Options:
    --minlength=8       Minimum password length
    --maxlength=8       Maximum password length
    --mintime=3600      Minimum mask runtime (seconds)
    --maxtime=3600      Maximum mask runtime (seconds)
    --mincomplexity=1   Minimum complexity
    --maxcomplexity=100
                        Maximum complexity
    --minoccurrence=1   Minimum occurrence
    --maxoccurrence=100
                        Maximum occurrence

  Mask Sorting Options:
    --optindex          sort by mask optindex (default)
    --occurrence        sort by mask occurrence
    --complexity        sort by mask complexity

  Check mask coverage:
    --checkmasks=?u?l?l?l?l?l?d,?l?l?l?l?l?d?d
                        check mask coverage
    --checkmasksfile=masks.hcmask
                        check mask coverage in a file

  Miscellaneous options:
    --pps=1000000000    Passwords per Second
    -q, --quiet         Don't show headers.

~~~
