# conchftp command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:   cftp [options] [user@]host
         cftp [options] [user@]host[:dir[/]]
         cftp [options] [user@]host[:file [localfile]]
Options:
  -V, --version                Display Twisted version and exit.
  -C, --compress               Enable compression.
  -v, --log                    Enable logging (defaults to stderr)
  -x, --nox11                  Disable X11 connection forwarding (default)
  -A, --agent                  Enable authentication agent forwarding
  -a, --noagent                Disable authentication agent forwarding (default)
  -r, --reconnect              Reconnect to the server if the connection is
                               lost.
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
  -B, --buffersize=            Size of the buffer to use for sending/receiving.
                               [default: 32768]
  -b, --batchfile=             File to read commands from, or '-' for stdin.
  -R, --requests=              Number of requests to make before waiting for a
                               reply. [default: 5]
  -s, --subsystem=             Subsystem/server program to connect to. [default:
                               sftp]
      --help                   Display this help and exit.

cftp is a client for logging into a remote machine and executing commands to
send and receive file information


~~~
