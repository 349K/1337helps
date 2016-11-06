# spd-conf command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: spd-conf [options]
A simple dialog based tool for basic configuration of Speech Dispatcher
and problem diagnostics.

Options:
  -h, --help            show this help message and exit
  -D, --debug           Debug a problem and generate a report
  -d, --diagnostics     Diagnose problems with the current setup
  --test-festival       Test whether Festival works as a server
  -C, --config-basic-settings-system
                        Configure basic settings in system-wide configuration
  --test-pulse          Test Pulse Audio
  -e, --espeak          Use espeak to synthesize messages
  -c, --config-basic-settings-user
                        Configure basic settings in user configuration
  -n, --dont-ask        Do not ask any questions, always use default values
  --test-espeak         Test whether Espeak works as a standalone binary
  -s, --test-spd-say    Test connection to Speech Dispatcher using spd-say
  -u, --create-user-conf
                        Create Speech Dispatcher configuration for the given
                        user
  --test-alsa           Test ALSA audio

~~~
