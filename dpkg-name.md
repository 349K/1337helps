# dpkg-name command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-name [<option>...] <file>...

Options:
  -a, --no-architecture    no architecture part in filename.
  -o, --overwrite          overwrite if file exists.
  -k, --symlink            don't create a new file, but a symlink.
  -s, --subdir [dir]       move file into subdirectory (use with care).
  -c, --create-dir         create target directory if not there (use with care).
  -?, --help               show this help message.
  -v, --version            show the version.

file.deb changes to <package>_<version>_<architecture>.<package_type>
according to the 'underscores convention'.

~~~
