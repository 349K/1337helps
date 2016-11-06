# dpkg-maintscript-helper command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-maintscript-helper <command> <parameter>... -- <maintainer-script-parameter>...

Commands:
  supports <command>
	Returns 0 (success) if the given command is supported, 1 otherwise.
  rm_conffile <conffile> [<last-version> [<package>]]
	Remove obsolete conffile. Must be called in preinst, postinst and
	postrm.
  mv_conffile <old-conf> <new-conf> [<last-version> [<package>]]
	Rename a conffile. Must be called in preinst, postinst and postrm.
  symlink_to_dir <pathname> <old-symlink-target> [<last-version> [<package>]]
	Replace a symlink with a directory. Must be called in preinst,
	postinst and postrm.
  dir_to_symlink <pathname> <new-symlink-target> [<last-version> [<package>]]
	Replace a directory with a symlink. Must be called in preinst,
	postinst and postrm.
  help
	Display this usage information.

~~~
