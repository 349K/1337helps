# snmpconf command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


/usr/bin/snmpconf [options] [FILETOCREATE...]
options:
  -f           overwrite existing files without prompting
  -i           install created files into /usr/share/snmp.
  -p           install created files into /root/.snmp.
  -I DIR       install created files into DIR.
  -a           Don't ask any questions, just read in current
                   current .conf files and comment them
  -r all|none  Read in all or none of the .conf files found.
  -R file,...  Read in a particular list of .conf files.
  -g GROUP     Ask a series of GROUPed questions.
  -G           List known GROUPs.
  -c conf_dir  use alternate configuration directory.
  -q           run more quietly with less advice.
  -d           turn on debugging output.
  -D           turn on debugging dumper output.

~~~
