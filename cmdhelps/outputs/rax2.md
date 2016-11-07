# rax2 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rax2 [options] [expr ...]
  =[base]                 ;  rax2 =10 0x46 -> output in base 10
  int   ->  hex           ;  rax2 10
  hex   ->  int           ;  rax2 0xa
  -int  ->  hex           ;  rax2 -77
  -hex  ->  int           ;  rax2 0xffffffb3
  int   ->  bin           ;  rax2 b30
  int   ->  ternary       ;  rax2 t42
  bin   ->  int           ;  rax2 1010d
  float ->  hex           ;  rax2 3.33f
  hex   ->  float         ;  rax2 Fx40551ed8
  oct   ->  hex           ;  rax2 35o
  hex   ->  oct           ;  rax2 Ox12 (O is a letter)
  bin   ->  hex           ;  rax2 1100011b
  hex   ->  bin           ;  rax2 Bx63
  hex   ->  ternary       ;  rax2 Tx23
  raw   ->  hex           ;  rax2 -S < /binfile
  hex   ->  raw           ;  rax2 -s 414141
  -b    binstr -> bin     ;  rax2 -b 01000101 01110110
  -B    keep base         ;  rax2 -B 33+3 -> 36
  -d    force integer     ;  rax2 -d 3 -> 3 instead of 0x3
  -e    swap endianness   ;  rax2 -e 0x33
  -f    floating point    ;  rax2 -f 6.3+2.1
  -F    stdin slurp C hex ;  rax2 -F < shellcode.c
  -h    help              ;  rax2 -h
  -k    randomart         ;  rax2 -k 0x34 1020304050
  -n    binary number     ;  rax2 -n 0x1234 # 34120000
  -N    binary number     ;  rax2 -N 0x1234 # \x34\x12\x00\x00
  -s    hexstr -> raw     ;  rax2 -s 43 4a 50
  -S    raw -> hexstr     ;  rax2 -S < /bin/ls > ls.hex
  -t    tstamp -> str     ;  rax2 -t 1234567890
  -x    hash string       ;  rax2 -x linux osx
  -u    units             ;  rax2 -u 389289238 # 317.0M
  -v    version           ;  rax2 -V

~~~
