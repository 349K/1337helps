# thc-pptp-bruter command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


thc-pptp-bruter [options] <remote host IP>
  -v        Verbose output / Debug output
  -W        Disable windows hack [default: enabled]
  -u <user> User [default: administrator]
  -w <file> Wordlist file [default: stdin]
  -p <n>    PPTP port [default: 1723]
  -n <n>    Number of parallel tries [default: 5]
  -l <n>    Limit to n passwords / sec [default: 100]

Windows-Hack reuses the LCP connection with the same caller-id. This
gets around MS's anti-brute forcing protection. It's enabled by default.

~~~
