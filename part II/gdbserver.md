# gdbserver command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:	gdbserver [OPTIONS] COMM PROG [ARGS ...]
	gdbserver [OPTIONS] --attach COMM PID
	gdbserver [OPTIONS] --multi COMM

COMM may either be a tty device (for serial debugging),
HOST:PORT to listen for a TCP connection, or '-' or 'stdio' to use 
stdin/stdout of gdbserver.
PROG is the executable program.  ARGS are arguments passed to inferior.
PID is the process ID to attach to, when --attach is specified.

Operating modes:

  --attach              Attach to running process PID.
  --multi               Start server without a specific program, and
                        only quit when explicitly commanded.
  --once                Exit after the first connection has closed.
  --help                Print this message and then exit.
  --version             Display version information and exit.

Other options:

  --wrapper WRAPPER --  Run WRAPPER to start new programs.
  --disable-randomization
                        Run PROG with address space randomization disabled.
  --no-disable-randomization
                        Don't disable address space randomization when
                        starting PROG.

Debug options:

  --debug               Enable general debugging output.
  --debug-format=opt1[,opt2,...]
                        Specify extra content in debugging output.
                          Options:
                            all
                            none
                            timestamp
  --remote-debug        Enable remote protocol debugging output.
  --disable-packet=opt1[,opt2,...]
                        Disable support for RSP packets or features.
                          Options:
                            vCont, Tthread, qC, qfThreadInfo and 
                            threads (disable all threading packets).

For more information, consult the GDB manual (available as on-line 
info or a printed manual).
Report bugs to "<http://www.gnu.org/software/gdb/bugs/>".

~~~
