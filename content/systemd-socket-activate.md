# systemd-socket-activate command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


systemd-socket-activate [OPTIONS...]

Listen on sockets and launch child on connection.

Options:
  -h --help                  Show this help and exit
     --version               Print version string and exit
  -l --listen=ADDR           Listen for raw connections at ADDR
  -d --datagram              Listen on datagram instead of stream socket
     --seqpacket             Listen on SOCK_SEQPACKET instead of stream socket
  -a --accept                Spawn separate child for each connection
  -E --setenv=NAME[=VALUE]   Pass an environment variable to children
     --fdname=NAME[:NAME...] Specify names for file descriptors
     --inetd                 Enable inetd file descriptor passing protocol

Note: file descriptors from sd_listen_fds() will be passed through.

~~~
