# gvfs-ls command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
  gvfs-ls [OPTION...] [LOCATION...]

List the contents of the locations.

Help Options:
  -?, --help                        Show help options

Application Options:
  -a, --attributes=ATTRIBUTES       The attributes to get
  -h, --hidden                      Show hidden files
  -l, --long                        Use a long listing format
  -c, --show-completions=PREFIX     Show completions
  -n, --nofollow-symlinks           Don't follow symbolic links
  -u, --print-uris                  Print full URIs
  --version                         Show program version

gvfs-ls is similar to the traditional ls utility, but using gvfs
locations instead of local files: for example you can use something
like smb://server/resource/file.txt as location. File attributes can
be specified with their gvfs name, e.g. standard::icon.

~~~
