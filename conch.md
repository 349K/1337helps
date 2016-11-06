# conch command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:   conch [options] host [command]
Options:
  -V, --version                Display Twisted version and exit.
  -C, --compress               Enable compression.
  -v, --log                    Enable logging (defaults to stderr)
  -x, --nox11                  Disable X11 connection forwarding (default)
  -A, --agent                  Enable authentication agent forwarding
  -a, --noagent                Disable authentication agent forwarding (default)
  -r, --reconnect              Reconnect to the server if the connection is
                               lost.
  -n, --null                   Redirect input from /dev/null.
  -f, --fork                   Fork to background after authentication.
  -t, --tty                    Tty; allocate a tty even if command is given.
  -T, --notty                  Do not allocate a tty.
  -N, --noshell                Do not execute a shell or command.
  -s, --subsystem              Invoke command (mandatory) as SSH2 subsystem.
  -l, --user=                  Log in using this user name.
  -i, --identity=              Identity for public-key authentication
  -c, --ciphers=               Select encryption algorithms
  -m, --macs=                  Specify MAC algorithms
  -p, --port=                  Connect to this port.  Server must be on the same
                               port.
  -o, --option=                Ignored OpenSSH options
      --host-key-algorithms=   Select host key algorithms
      --known-hosts=           File to check for host keys
      --user-authentications=  Choose how to authenticate to the remote server
      --logfile=               File to log to, or - for stdout
  -e, --escape=                Set escape character; ``none'' = disable
                               [default: ~]
  -L, --localforward=          Forward local port to remote address
                               (lport:host:port)
  -R, --remoteforward=         Forward remote port to local address
                               (rport:host:port)
      --help                   Display this help and exit.

conch is a SSHv2 client that allows logging into a remote machine and executing
commands.


~~~
