# mpg123-pulse command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

High Performance MPEG 1.0/2.0/2.5 Audio Player for Layers 1, 2 and 3
	version 1.22.4; written and copyright by Michael Hipp and others
	free software (LGPL) without any warranty but with best wishes

usage: mpg123.bin [option(s)] [file(s) | URL(s) | -]
supported options [defaults in brackets]:
   -v    increase verbosity level       -q    quiet (don't print title)
   -t    testmode (no output)           -s    write to stdout
   -w f  write output as WAV file
   -k n  skip first n frames [0]        -n n  decode only n frames [all]
   -c    check range violations         -y    DISABLE resync on errors
   -b n  output buffer: n Kbytes [0]    -f n  change scalefactor [32768]
   -r n  set/force samplerate [auto]
   -o m  select output module           -a d  set audio device
   -2    downsample 1:2 (22 kHz)        -4    downsample 1:4 (11 kHz)
   -d n  play every n'th frame only     -h n  play every frame n times
   -0    decode channel 0 (left) only   -1    decode channel 1 (right) only
   -m    mix both channels (mono)       -p p  use HTTP proxy p [$HTTP_PROXY]
   -@ f  read filenames/URLs from f     -T get realtime priority
   -z    shuffle play (with wildcards)  -Z    random play
   -u a  HTTP authentication string     -E f  Equalizer, data from file
   -C    enable control keys            --no-gapless  not skip junk/padding in mp3s
   -?    this help                      --version  print name + version
See the manpage mpg123(1) or call mpg123.bin with --longhelp for more parameters and information.

~~~
