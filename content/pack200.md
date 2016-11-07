# pack200 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:  pack200 [-opt... | --option=value]... x.pack[.gz] y.jar

Packing Options
  -g, --no-gzip                   output a plain *.pack file with no zipping
  --gzip                          (default) post-process the pack output with gzip
  -G, --strip-debug               remove debugging attributes while packing
  -O, --no-keep-file-order        do not transmit file ordering information
  --keep-file-order               (default) preserve input file ordering
  -S{N}, --segment-limit={N}      output segment limit (default N=1Mb)
  -E{N}, --effort={N}             packing effort (default N=5)
  -H{h}, --deflate-hint={h}       transmit deflate hint: true, false, or keep (default)
  -m{V}, --modification-time={V}  transmit modtimes: latest or keep (default)
  -P{F}, --pass-file={F}          transmit the given input element(s) uncompressed
  -U{a}, --unknown-attribute={a}  unknown attribute action: error, strip, or pass (default)
  -C{N}={L}, --class-attribute={N}={L}  (user-defined attribute)
  -F{N}={L}, --field-attribute={N}={L}  (user-defined attribute)
  -M{N}={L}, --method-attribute={N}={L} (user-defined attribute)
  -D{N}={L}, --code-attribute={N}={L}   (user-defined attribute)
  -f{F}, --config-file={F}        read file F for Pack200.Packer properties
  -v, --verbose                   increase program verbosity
  -q, --quiet                     set verbosity to lowest level
  -l{F}, --log-file={F}           output to the given log file, or '-' for System.out
  -?, -h, --help                  print this message
  -V, --version                   print program version
  -J{X}                           pass option X to underlying Java VM

Notes:
  The -P, -C, -F, -M, and -D options accumulate.
  Example attribute definition:  -C SourceFile=RUH .
  Config. file properties are defined by the Pack200 API.
  For meaning of -S, -E, -H-, -m, -U values, see Pack200 API.
  Layout definitions (like RUH) are defined by JSR 200.

Repacking mode updates the JAR file with a pack/unpack cycle:
    pack200 [-r|--repack] [-opt | --option=value]... [repackedy.jar] y.jar


~~~
