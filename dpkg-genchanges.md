# dpkg-genchanges command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-genchanges [<option>...]

Options:
  --build=<type>[,...]     specify the build <type>: full, source, binary,
                             any, all (default is 'full').
  -g                       source and arch-indep build.
  -G                       source and arch-specific build.
  -b                       binary-only, no source files.
  -B                       binary-only, only arch-specific files.
  -A                       binary-only, only arch-indep files.
  -S                       source-only, no binary files.
  -c<control-file>         get control info from this file.
  -l<changelog-file>       get per-version info from this file.
  -f<files-list-file>      get .deb files list from this file.
  -v<since-version>        include all changes later than version.
  -C<changes-description>  use change description from this file.
  -m<maintainer>           override control's maintainer value.
  -e<maintainer>           override changelog's maintainer value.
  -u<upload-files-dir>     directory with files (default is '..').
  -si                      source includes orig, if new upstream (default).
  -sa                      source includes orig, always.
  -sd                      source is diff and .dsc only.
  -q                       quiet - no informational messages on stderr.
  -F<changelog-format>     force changelog format.
  -V<name>=<value>         set a substitution variable.
  -T<substvars-file>       read variables here, not debian/substvars.
  -D<field>=<value>        override or add a field and value.
  -U<field>                remove a field.
  -O[<filename>]           write to stdout (default) or <filename>.
  -?, --help               show this help message.
      --version            show the version.

~~~
