# rabin2 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rabin2 [-ACdehHiIjlLMqrRsSvVxzZ] [-@ addr] [-a arch] [-b bits]
              [-B addr] [-c F:C:D] [-f str] [-m addr] [-n str] [-N m:M]
              [-o str] [-O str] [-k query] [-D lang symname] | file>
 -@ [addr]       show section, symbol or import at addr
 -A              list archs
 -a [arch]       set arch (x86, arm, .. or <arch>_<bits>)
 -b [bits]       set bits (32, 64 ...)
 -B [addr]       override base address (pie bins)
 -c [fmt:C:D]    create [elf,mach0,pe] with Code and Data hexpairs (see -a)
 -C              list classes
 -d              show debug/dwarf information
 -D lang name    demangle symbol name
 -e              entrypoint
 -E              show loading offset (useful for non-ASLR libraries) -f [str]        select sub-bin named str
 -F [binfmt]     force to use that bin plugin (ignore header check)
 -k [query]      perform sdb query on loaded file
 -K [algo]       calculate checksums (md5, sha1, ..)
 -g              same as -SMResiz (show all info)
 -G [addr]       load address . offset to header
 -h              this help
 -H              header fields
 -i              imports (symbols imported from libraries)
 -I              binary info
 -j              output in json
 -k [sdb-query]  run sdb query. for example: '*'
 -l              linked libraries
 -L              list supported bin plugins
 -m [addr]       show source line at addr
 -M              main (show address of main symbol)
 -n [str]        show section, symbol or import named str
 -N [min:max]    force min:max number of chars per string (see -z and -zz)
 -o [str]        output file/folder for write operations (out by default)
 -O [str]        write/extract operations (-O help)
 -p              show physical addresses
 -P              show debug/pdb information
 -PP             download pdb file for binary
 -q              be quiet, just show fewer data
 -r              radare output
 -R              relocations
 -s              symbols (exports)
 -S              sections
 -v              display version and quit
 -x              extract bins contained in file
 -z              strings (from data section)
 -zz             strings (from raw bins [e bin.rawstr=1])
 -zzz            dump raw strings to stdout (for huge files)
 -Z              guess size of binary program

~~~
