# dpkg-split command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-split [<option> ...] <command>

Commands:
  -s|--split <file> [<prefix>]     Split an archive.
  -j|--join <part> <part> ...      Join parts together.
  -I|--info <part> ...             Display info about a part.
  -a|--auto -o <complete> <part>   Auto-accumulate parts.
  -l|--listq                       List unmatched pieces.
  -d|--discard [<filename> ...]    Discard unmatched pieces.

  -?, --help                       Show this help message.
      --version                    Show the version.

Options:
  --depotdir <directory>           Use <directory> instead of /var/lib/dpkg/parts.
  -S|--partsize <size>             In KiB, for -s (default is 450).
  -o|--output <file>               Filename, for -j (default is
                                     <package>_<version>_<arch>.deb).
  -Q|--npquiet                     Be quiet when -a is not a part.
  --msdos                          Generate 8.3 filenames.

Exit status:
  0 = ok
  1 = with --auto, file is not a part
  2 = trouble

~~~
