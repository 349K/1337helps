# couchdb command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: couchdb [OPTION]

The couchdb command runs the Apache CouchDB server.

Erlang is called with:

    -os_mon     start_memsup false     start_cpu_sup false     disk_space_check_interval 1     disk_almost_full_threshold 1 -sasl errlog_type error +K true +A 4

Erlang inherits the environment of this command.

You can override these options using the environment:

    ERL_AFLAGS, ERL_FLAGS, ERL_ZFLAGS

See erl(1) for more information about the environment variables.

The exit status is 0 for success or 1 for failure.

Options:

  -h          display a short help message and exit
  -V          display version information and exit
  -a FILE     add configuration FILE to chain
  -A DIR      add configuration DIR to chain
  -n          reset configuration file chain (including system default)
  -c          print configuration file chain and exit
  -i          use the interactive Erlang shell
  -b          spawn as a background process
  -p FILE     set the background PID FILE (overrides system default)
  -r SECONDS  respawn background process after SECONDS (defaults to no respawn)
  -o FILE     redirect background stdout to FILE (defaults to couchdb.stdout)
  -e FILE     redirect background stderr to FILE (defaults to couchdb.stderr)
  -s          display the status of the background process
  -k          kill the background process, will respawn if needed
  -d          shutdown the background process

Report bugs at <https://issues.apache.org/jira/browse/COUCHDB>.

~~~
