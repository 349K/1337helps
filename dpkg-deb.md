# dpkg-deb command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-deb [<option> ...] <command>

Commands:
  -b|--build <directory> [<deb>]   Build an archive.
  -c|--contents <deb>              List contents.
  -I|--info <deb> [<cfile> ...]    Show info to stdout.
  -W|--show <deb>                  Show information on package(s)
  -f|--field <deb> [<cfield> ...]  Show field(s) to stdout.
  -e|--control <deb> [<directory>] Extract control info.
  -x|--extract <deb> <directory>   Extract files.
  -X|--vextract <deb> <directory>  Extract & list files.
  -R|--raw-extract <deb> <directory>
                                   Extract control info and files.
  --ctrl-tarfile <deb>             Output control tarfile.
  --fsys-tarfile <deb>             Output filesystem tarfile.

  -?, --help                       Show this help message.
      --version                    Show the version.

<deb> is the filename of a Debian format archive.
<cfile> is the name of an administrative file component.
<cfield> is the name of a field in the main 'control' file.

Options:
  -v, --verbose                    Enable verbose output.
  -D, --debug                      Enable debugging output.
      --showformat=<format>        Use alternative format for --show.
      --deb-format=<format>        Select archive format.
                                     Allowed values: 0.939000, 2.0 (default).
      --old                        Legacy alias for '--deb-format=0.939000'.
      --new                        Legacy alias for '--deb-format=2.0'.
      --nocheck                    Suppress control file check (build bad
                                     packages).
      --uniform-compression        Use the compression params on all members.
  -z#                              Set the compression level when building.
  -Z<type>                         Set the compression type used when building.
                                     Allowed types: gzip, xz, bzip2, none.
  -S<strategy>                     Set the compression strategy when building.
                                     Allowed values: none; extreme (xz);
                                     filtered, huffman, rle, fixed (gzip).

Format syntax:
  A format is a string that will be output for each package. The format
  can include the standard escape sequences \n (newline), \r (carriage
  return) or \\ (plain backslash). Package information can be included
  by inserting variable references to package fields using the ${var[;width]}
  syntax. Fields will be right-aligned unless the width is negative in which
  case left alignment will be used.

Use 'dpkg' to install and remove packages from your system, or
'apt' or 'aptitude' for user-friendly package management. Packages
unpacked using 'dpkg-deb --extract' will be incorrectly installed !

~~~
