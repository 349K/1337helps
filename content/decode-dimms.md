# decode-dimms command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: /usr/bin/decode-dimms [-c] [-f [-b]] [-x|-X file [files..]]
       /usr/bin/decode-dimms -h

  -f, --format            Print nice html output
  -b, --bodyonly          Don't print html header
                          (useful for postprocessing the output)
      --side-by-side      Display all DIMMs side-by-side if possible
      --merge-cells       Merge neighbour cells with identical values
                          (side-by-side output only)
  -c, --checksum          Decode completely even if checksum fails
  -x,                     Read data from hexdump files
  -X,                     Same as -x except treat multibyte hex
                          data as little endian
  -h, --help              Display this usage summary

Hexdumps can be the output from hexdump, hexdump -C, i2cdump, eeprog and
likely many other progams producing hex dumps of one kind or another.  Note
that the default output of "hexdump" will be byte-swapped on little-endian
systems and you must use -X instead of -x, otherwise the dump will not be
parsed correctly.  It is better to use "hexdump -C", which is not ambiguous.

~~~
