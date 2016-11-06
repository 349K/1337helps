# clusterd command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

[32m
		clusterd/0.5 - clustered attack toolkit[0m
			[33m[Supporting 7 platforms][0m

usage: ./clusterd.py [options]

optional arguments:
  -h, --help            show this help message and exit

Connection:
  Options for configuring the connection

  -i [ip address]       Server address
  -iL [file]            Server list
  -p [port]             Server port
  --proxy [proxy://server:port]
                        Connect through proxy [http|https]
  --proxy-auth [username:password]
                        Proxy credentials
  --timeout [seconds]   Connection timeout [5s]
  --random-agent        Use a random User-Agent for requests
  --ssl                 Force SSL

Remote Host:
  Settings specific to the remote host

  -a [jboss|coldfusion|weblogic|tomcat|railo|axis2|glassfish]
                        Hint at remote host service
  -o [windows|linux]    Hint at remote host OS
  -v [version]          Specific version to test
  --usr-auth [username:password]
                        Login credentials for service
  --fingerprint         Fingerprint the remote system
  --arch [x86|x64]      Specify remote OS architecture
  --delay [seconds]     Delay N seconds between each attempt

Deploy:
  Deployment flags and settings

  --deploy [file]       Deploy to the discovered service
  --undeploy [context]  Undeploy file from server
  --deployer [deployer]
                        Specify a deployer to use
  --invoke              Invoke payload after deployment
  --rand-payload        Use a random name for the deployed file
  -b [user]             Brute force credentials for user [admin]
  --wordlist [path]     Wordlist for brute forcing passwords

Other:
  Miscellaneous flags

  --deployer-list [platform]
                        List all available deployers
  --aux-list [platform]
                        List all available exploits
  --gen-payload [host:port] for reverse connection
                        Generate a reverse shell payload
  --discover [discovery_file]
                        Attempt to discover application servers using the
                        specified nmap gnmap output (use -sV when scanning)
  --listen [adapter]    Adapter to listen on when needed
  -d                    Enable debug output
  -l                    Log output to file [$time$_log.log]

~~~
