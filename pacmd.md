# pacmd command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


pacmd exit
pacmd help
pacmd list-(modules|sinks|sources|clients|cards|samples)
pacmd list-(sink-inputs|source-outputs)
pacmd stat
pacmd info
pacmd load-module NAME [ARGS ...]
pacmd unload-module NAME|#N
pacmd describe-module NAME
pacmd set-(sink|source)-volume NAME|#N VOLUME
pacmd set-(sink-input|source-output)-volume #N VOLUME
pacmd set-(sink|source)-mute NAME|#N 1|0
pacmd set-(sink-input|source-output)-mute #N 1|0
pacmd update-(sink|source)-proplist NAME|#N KEY=VALUE
pacmd update-(sink-input|source-output)-proplist #N KEY=VALUE
pacmd set-default-(sink|source) NAME|#N
pacmd kill-(client|sink-input|source-output) #N
pacmd play-sample NAME SINK|#N
pacmd remove-sample NAME
pacmd load-sample NAME FILENAME
pacmd load-sample-lazy NAME FILENAME
pacmd load-sample-dir-lazy PATHNAME
pacmd play-file FILENAME SINK|#N
pacmd dump
pacmd move-(sink-input|source-output) #N SINK|SOURCE
pacmd suspend-(sink|source) NAME|#N 1|0
pacmd suspend 1|0
pacmd set-card-profile CARD PROFILE
pacmd set-(sink|source)-port NAME|#N PORT
pacmd set-port-latency-offset CARD-NAME|CARD-#N PORT OFFSET
pacmd set-log-target TARGET
pacmd set-log-level NUMERIC-LEVEL
pacmd set-log-meta 1|0
pacmd set-log-time 1|0
pacmd set-log-backtrace FRAMES

  -h, --help                            Show this help
      --version                         Show version
When no command is given pacmd starts in the interactive mode.

~~~
