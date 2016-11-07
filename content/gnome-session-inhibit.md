# gnome-session-inhibit command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


gnome-session-inhibit [OPTION...] COMMAND

Execute COMMAND while inhibiting some session functionality.

  -h, --help        Show this help
  --version         Show program version
  --app-id ID       The application id to use
                    when inhibiting (optional)
  --reason REASON   The reason for inhibiting (optional)
  --inhibit ARG     Things to inhibit, colon-separated list of:
                    logout, switch-user, suspend, idle, automount
  --inhibit-only    Do not launch COMMAND and wait forever instead

If no --inhibit option is specified, idle is assumed.

~~~
