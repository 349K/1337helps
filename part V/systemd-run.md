# systemd-run command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


systemd-run [OPTIONS...] {COMMAND} [ARGS...]

Run the specified command in a transient scope or service or timer
unit. If a timer option is specified and the unit specified with
the --unit option exists, the command can be omitted.

  -h --help                       Show this help
     --version                    Show package version
     --no-ask-password            Do not prompt for password
     --user                       Run as user unit
  -H --host=[USER@]HOST           Operate on remote host
  -M --machine=CONTAINER          Operate on local container
     --scope                      Run this as scope rather than service
     --unit=UNIT                  Run under the specified unit name
  -p --property=NAME=VALUE        Set unit property
     --description=TEXT           Description for unit
     --slice=SLICE                Run in the specified slice
     --no-block                   Do not wait until operation finished
  -r --remain-after-exit          Leave service around until explicitly stopped
     --send-sighup                Send SIGHUP when terminating
     --service-type=TYPE          Service type
     --uid=USER                   Run as system user
     --gid=GROUP                  Run as system group
     --nice=NICE                  Nice level
  -E --setenv=NAME=VALUE          Set environment
  -t --pty                        Run service on pseudo tty
  -q --quiet                      Suppress information messages during runtime

Timer options:

     --on-active=SECONDS          Run after SECONDS delay
     --on-boot=SECONDS            Run SECONDS after machine was booted up
     --on-startup=SECONDS         Run SECONDS after systemd activation
     --on-unit-active=SECONDS     Run SECONDS after the last activation
     --on-unit-inactive=SECONDS   Run SECONDS after the last deactivation
     --on-calendar=SPEC           Realtime timer
     --timer-property=NAME=VALUE  Set timer unit property

~~~
