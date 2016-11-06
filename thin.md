# thin command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: thin [options] start|stop|restart|config|install

Server options:
    -a, --address HOST               bind to HOST address (default: 0.0.0.0)
    -p, --port PORT                  use PORT (default: 3000)
    -S, --socket FILE                bind to unix domain socket
    -y, --swiftiply [KEY]            Run using swiftiply
    -A, --adapter NAME               Rack adapter to use (default: autodetect)
                                     (rack, rails, ramaze, merb, file)
    -R, --rackup FILE                Load a Rack config file instead of Rack adapter
    -c, --chdir DIR                  Change to dir before starting
        --stats PATH                 Mount the Stats adapter under PATH

SSL options:
        --ssl                        Enables SSL
        --ssl-key-file PATH          Path to private key
        --ssl-cert-file PATH         Path to certificate
        --ssl-disable-verify         Disables (optional) client cert requests

Adapter options:
    -e, --environment ENV            Framework environment (default: development)
        --prefix PATH                Mount the app under PATH (start with /)

Daemon options:
    -d, --daemonize                  Run daemonized in the background
    -l, --log FILE                   File to redirect output (default: /root/helps/log/thin.log)
    -P, --pid FILE                   File to store PID (default: tmp/pids/thin.pid)
    -u, --user NAME                  User to run daemon as (use with -g)
    -g, --group NAME                 Group to run daemon as (use with -u)
        --tag NAME                   Additional text to display in process listing

Cluster options:
    -s, --servers NUM                Number of servers to start
    -o, --only NUM                   Send command to only one server of the cluster
    -C, --config FILE                Load options from config file
        --all [DIR]                  Send command to each config files in DIR
    -O, --onebyone                   Restart the cluster one by one (only works with restart command)
    -w, --wait NUM                   Maximum wait time for server to be started in seconds (use with -O)

Tuning options:
    -b, --backend CLASS              Backend to use, full classname
    -t, --timeout SEC                Request or command timeout in sec (default: 30)
    -f, --force                      Force the execution of the command
        --max-conns NUM              Maximum number of open file descriptors (default: 1024)
                                     Might require sudo to set higher than 1024
        --max-persistent-conns NUM   Maximum number of persistent connections
                                     (default: 100)
        --threaded                   Call the Rack application in threads [experimental]
        --threadpool-size NUM        Sets the size of the EventMachine threadpool.
                                     (default: 20)
        --no-epoll                   Disable the use of epoll

Common options:
    -r, --require FILE               require the library
    -q, --quiet                      Silence all logging
    -D, --debug                      Enable debug logging
    -V, --trace                      Set tracing on (log raw request/response)
    -h, --help                       Show this message
    -v, --version                    Show version

~~~
