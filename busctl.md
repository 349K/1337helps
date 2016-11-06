# busctl command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


busctl [OPTIONS...] {COMMAND} ...

Introspect the bus.

  -h --help               Show this help
     --version            Show package version
     --no-pager           Do not pipe output into a pager
     --no-legend          Do not show the headers and footers
     --system             Connect to system bus
     --user               Connect to user bus
  -H --host=[USER@]HOST   Operate on remote host
  -M --machine=CONTAINER  Operate on local container
     --address=ADDRESS    Connect to bus specified by address
     --show-machine       Show machine ID column in list
     --unique             Only show unique names
     --acquired           Only show acquired names
     --activatable        Only show activatable names
     --match=MATCH        Only show matching messages
     --size=SIZE          Maximum length of captured packet
     --list               Don't show tree, but simple object path list
     --quiet              Don't show method call reply
     --verbose            Show result values in long format
     --expect-reply=BOOL  Expect a method call reply
     --auto-start=BOOL    Auto-start destination service
     --allow-interactive-authorization=BOOL
                          Allow interactive authorization for operation
     --timeout=SECS       Maximum time to wait for method call completion
     --augment-creds=BOOL Extend credential data with data read from /proc/$PID

Commands:
  list                    List bus names
  status [SERVICE]        Show bus service, process or bus owner credentials
  monitor [SERVICE...]    Show bus traffic
  capture [SERVICE...]    Capture bus traffic as pcap
  tree [SERVICE...]       Show object tree of service
  introspect SERVICE OBJECT [INTERFACE]
  call SERVICE OBJECT INTERFACE METHOD [SIGNATURE [ARGUMENT...]]
                          Call a method
  get-property SERVICE OBJECT INTERFACE PROPERTY...
                          Get property value
  set-property SERVICE OBJECT INTERFACE PROPERTY SIGNATURE ARGUMENT...
                          Set property value
  help                    Show this help

~~~
