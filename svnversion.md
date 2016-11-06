# svnversion command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: svnversion [OPTIONS] [WC_PATH [TRAIL_URL]]
Subversion working copy identification tool.
Type 'svnversion --version' to see the program version.

  Produce a compact version identifier for the working copy path
  WC_PATH.  TRAIL_URL is the trailing portion of the URL used to
  determine if WC_PATH itself is switched (detection of switches
  within WC_PATH does not rely on TRAIL_URL).  The version identifier
  is written to standard output.  For example:

    $ svnversion . /repos/svn/trunk
    4168

  The version identifier will be a single number if the working
  copy is single revision, unmodified, not switched and with
  a URL that matches the TRAIL_URL argument.  If the working
  copy is unusual the version identifier will be more complex:

   4123:4168     mixed revision working copy
   4168M         modified working copy
   4123S         switched working copy
   4123P         partial working copy, from a sparse checkout
   4123:4168MS   mixed revision, modified, switched working copy

  If WC_PATH is an unversioned path, the program will output
  'Unversioned directory' or 'Unversioned file'.  If WC_PATH is
  an added or copied or moved path, the program will output
  'Uncommitted local addition, copy or move'.

  If invoked without arguments WC_PATH will be the current directory.

Valid options:
  -n [--no-newline]        : do not output the trailing newline
  -c [--committed]         : last changed rather than current revisions
  -h [--help]              : display this help
  --version                : show program version information
  -q [--quiet]             : no progress (only errors) to stderr


~~~
