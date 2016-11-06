# jdb command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

invalid option: --help

Usage: jdb <options> <class> <arguments>

where options include:
    -help             print out this message and exit
    -sourcepath <directories separated by ":">
                      directories in which to look for source files
    -attach <address>
                      attach to a running VM at the specified address using standard connector
    -listen <address>
                      wait for a running VM to connect at the specified address using standard connector
    -listenany
                      wait for a running VM to connect at any available address using standard connector
    -launch
                      launch VM immediately instead of waiting for 'run' command
    -listconnectors   list the connectors available in this VM
    -connect <connector-name>:<name1>=<value1>,...
                      connect to target VM using named connector with listed argument values
    -dbgtrace [flags] print info for debugging jdb
    -tclient          run the application in the HotSpot(TM) Client Compiler
    -tserver          run the application in the HotSpot(TM) Server Compiler

options forwarded to debuggee process:
    -v -verbose[:class|gc|jni]
                      turn on verbose mode
    -D<name>=<value>  set a system property
    -classpath <directories separated by ":">
                      list directories in which to look for classes
    -X<option>        non-standard target VM option

<class> is the name of the class to begin debugging
<arguments> are the arguments passed to the main() method of <class>

For command help type 'help' at jdb prompt

~~~
