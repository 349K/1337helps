# pactl command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


pactl [options] stat
pactl [options] info
pactl [options] list [short] [TYPE]
pactl [options] exit
pactl [options] upload-sample FILENAME [NAME]
pactl [options] play-sample  NAME [SINK]
pactl [options] remove-sample  NAME
pactl [options] load-module  NAME [ARGS ...]
pactl [options] unload-module  NAME|#N
pactl [options] move-(sink-input|source-output) #N SINK|SOURCE
pactl [options] suspend-(sink|source) NAME|#N 1|0
pactl [options] set-card-profile  CARD PROFILE
pactl [options] set-default-(sink|source) NAME
pactl [options] set-(sink|source)-port NAME|#N PORT
pactl [options] set-(sink|source)-volume NAME|#N VOLUME [VOLUME ...]
pactl [options] set-(sink-input|source-output)-volume #N VOLUME [VOLUME ...]
pactl [options] set-(sink|source)-mute NAME|#N 1|0|toggle
pactl [options] set-(sink-input|source-output)-mute #N 1|0|toggle
pactl [options] set-sink-formats #N FORMATS
pactl [options] set-port-latency-offset CARD-NAME|CARD-#N PORT OFFSET
pactl [options] subscribe

The special names @DEFAULT_SINK@, @DEFAULT_SOURCE@ and @DEFAULT_MONITOR@
can be used to specify the default sink, source and monitor.

  -h, --help                            Show this help
      --version                         Show version

  -s, --server=SERVER                   The name of the server to connect to
  -n, --client-name=NAME                How to call this client on the server

~~~
