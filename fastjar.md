# fastjar command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: fastjar {ctxuV}[vfm0ME@] [jar-file] [manifest-file] [-C dir] files ...

Store many files together in a single `jar' file.

  -c              create new archive
  -t              list table of contents for archive
  -x              extract named (or all) files from archive
  -u              update existing archive

  -@              read names from stdin
  -0              store only; use no ZIP compression
  -C DIR FILE     change to the specified directory and include
                  the following file
  -E              don't include the files found in a directory
  -f FILE         specify archive file name
  --help          print this help, then exit
  -m FILE         include manifest information from specified manifest file
  -M              Do not create a manifest file for the entries
  -i              generate an index of the packages in this jar
                  and its Class-Path (currently unimplemented)
  -v              generate verbose output on standard output
  -V, --version   display version information

  -J*             -J options are ignored
  @FILE           expand options and files from FILE

If any file is a directory then it is processed recursively.
The manifest file name and the archive file name needs to be specified
in the same order the 'm' and 'f' flags are specified.

Example 1: to archive two class files into an archive called classes.jar: 
     jar cvf classes.jar Foo.class Bar.class 
Example 2: use an existing manifest file 'mymanifest' and archive all the
     files in the foo/ directory into 'classes.jar': 
     jar cvfm classes.jar mymanifest -C foo/ .

~~~
