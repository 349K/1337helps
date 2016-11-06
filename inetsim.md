# inetsim command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

INetSim 1.2.5 (2014-05-24) by Matthias Eckert & Thomas Hungenberg

Usage: ./inetsim [options]

Available options:
  --help                         Print this help message.
  --version                      Show version information.
  --config=<filename>            Configuration file to use.
  --log-dir=<directory>          Directory logfiles are written to.
  --data-dir=<directory>         Directory containing service data.
  --report-dir=<directory>       Directory reports are written to.
  --bind-address=<IP address>    Default IP address to bind services to.
                                 Overrides configuration option 'default_bind_address'.
  --max-childs=<num>             Default maximum number of child processes per service.
                                 Overrides configuration option 'default_max_childs'.
  --user=<username>              Default user to run services.
                                 Overrides configuration option 'default_run_as_user'.
  --faketime-init-delta=<secs>   Initial faketime delta (seconds).
                                 Overrides configuration option 'faketime_init_delta'.
  --faketime-auto-delay=<secs>   Delay for auto incrementing faketime (seconds).
                                 Overrides configuration option 'faketime_auto_delay'.
  --faketime-auto-incr=<secs>    Delta for auto incrementing faketime (seconds).
                                 Overrides configuration option 'faketime_auto_increment'.
  --session=<id>                 Session id to use. Defaults to main process id.
  --pidfile=<filename>           Pid file to use. Defaults to '/var/run/inetsim.pid'.


~~~
