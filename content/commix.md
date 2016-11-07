# commix command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: python commix.py [option(s)]

Options:
  -h, --help            Show help and exit.

  [1mGeneral[0m:
    These options relate to general matters.

    -v VERBOSE          Verbosity level (0-1, Default: 0).
    --version           Show version number and exit.
    --output-dir=OUT..  Set custom output directory path.
    -s SESSION_FILE     Load session from a stored (.sqlite) file.
    --flush-session     Flush session files for current target.
    --ignore-session    Ignore results stored in session file.

  [1mTarget[0m:
    This options has to be provided, to define the target URL.

    -u URL, --url=URL   Target URL.
    --url-reload        Reload target URL after command execution.
    -l LOGFILE          Parse target and data from HTTP proxy log file.
    --crawl=CRAWLDEPTH  Crawl the website starting from the target URL (1-2,
                        Default: 0).

  [1mRequest[0m:
    These options can be used to specify how to connect to the target URL.

    --data=DATA         Data string to be sent through POST.
    --host=HOST         HTTP Host header.
    --referer=REFERER   HTTP Referer header.
    --user-agent=AGENT  HTTP User-Agent header.
    --random-agent      Use a randomly selected HTTP User-Agent header.
    --param-del=PDEL    Set character for splitting parameter values.
    --cookie=COOKIE     HTTP Cookie header.
    --cookie-del=CDEL   Set character for splitting cookie values.
    --headers=HEADERS   Extra headers (e.g. 'Header1:Value1\nHeader2:Value2').
    --proxy=PROXY       Use a HTTP proxy (e.g. '127.0.0.1:8080').
    --tor               Use the Tor network.
    --tor-port=TOR_P..  Set Tor proxy port (Default: 8118).
    --auth-url=AUTH_..  Login panel URL.
    --auth-data=AUTH..  Login parameters and data.
    --auth-type=AUTH..  HTTP authentication type (e.g. 'Basic' or 'Digest').
    --auth-cred=AUTH..  HTTP authentication credentials (e.g. 'admin:admin').
    --ignore-401        Ignore HTTP error 401 (Unauthorized).
    --force-ssl         Force usage of SSL/HTTPS.

  [1mEnumeration[0m:
    These options can be used to enumerate the target host.

    --all               Retrieve everything.
    --current-user      Retrieve current user name.
    --hostname          Retrieve current hostname.
    --is-root           Check if the current user have root privileges.
    --is-admin          Check if the current user have admin privileges.
    --sys-info          Retrieve system information.
    --users             Retrieve system users.
    --passwords         Retrieve system users password hashes.
    --privileges        Retrieve system users privileges.
    --ps-version        Retrieve PowerShell's version number.

  [1mFile access[0m:
    These options can be used to access files on the target host.

    --file-read=FILE..  Read a file from the target host.
    --file-write=FIL..  Write to a file on the target host.
    --file-upload=FI..  Upload a file on the target host.
    --file-dest=FILE..  Host's absolute filepath to write and/or upload to.

  [1mModules[0m:
    These options can be used increase the detection and/or injection
    capabilities.

    --icmp-exfil=IP_..  The 'ICMP exfiltration' injection module.
                        (e.g. 'ip_src=192.168.178.1,ip_dst=192.168.178.3').
    --dns-server=DNS..  The 'DNS exfiltration' injection module.
                        (Domain name used for DNS exfiltration attack).
    --shellshock        The 'shellshock' injection module.

  [1mInjection[0m:
    These options can be used to specify which parameters to inject and to
    provide custom injection payloads.

    -p TEST_PARAMETER   Testable parameter(s).
    --suffix=SUFFIX     Injection payload suffix string.
    --prefix=PREFIX     Injection payload prefix string.
    --technique=TECH    Specify injection technique(s) to use.
    --maxlen=MAXLEN     Set the max length of output for time-related
                        injection techniques (Default: 10000 chars).
    --delay=DELAY       Set custom time delay for time-related injection
                        techniques (Default: 1 sec).
    --tmp-path=TMP_P..  Set the absolute path of web server's temp directory.
    --root-dir=SRV_R..  Set the absolute path of web server's root directory.
    --alter-shell=AL..  Use an alternative os-shell (e.g. 'Python').
    --os-cmd=OS_CMD     Execute a single operating system command.
    --os=OS             Force back-end operating system to this value.
    --tamper=TAMPER     Use given script(s) for tampering injection data.

  [1mDetection[0m:
    These options can be used to customize the detection phase.

    --level=LEVEL       Level of tests to perform (1-3, Default: 1).
    --skip-calc         Skip the mathematic calculation during the detection
                        phase.

  [1mMiscellaneous[0m:
    --dependencies      Check for third-party (non-core) dependencies.
    --skip-waf          Skip heuristic detection of WAF/IPS/IDS protection.

~~~
