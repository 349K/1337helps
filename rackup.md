# rackup command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rackup [ruby options] [rack options] [rackup config]

Ruby options:
  -e, --eval LINE          evaluate a LINE of code
  -b BUILDER_LINE,         evaluate a BUILDER_LINE of code as a builder script
      --builder
  -d, --debug              set debugging flags (set $DEBUG to true)
  -w, --warn               turn warnings on for your script
  -q, --quiet              turn off logging
  -I, --include PATH       specify $LOAD_PATH (may be used more than once)
  -r, --require LIBRARY    require the library, before executing your script

Rack options:
  -s, --server SERVER      serve using SERVER (thin/puma/webrick/mongrel)
  -o, --host HOST          listen on HOST (default: localhost)
  -p, --port PORT          use PORT (default: 9292)
  -O NAME[=VALUE],         pass VALUE to the server as option NAME. If no VALUE, sets it to true. Run '/usr/bin/rackup -s SERVER -h' to get a list of options for SERVER
      --option
  -E, --env ENVIRONMENT    use ENVIRONMENT for defaults (default: development)
  -D, --daemonize          run daemonized in the background
  -P, --pid FILE           file to store PID

Common options:
  -h, -?, --help           Show this message
      --version            Show version


~~~
