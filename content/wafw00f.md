# wafw00f command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


                                 ^     ^
        _   __  _   ____ _   __  _    _   ____
       ///7/ /.' \ / __////7/ /,' \ ,' \ / __/
      | V V // o // _/ | V V // 0 // 0 // _/
      |_n_,'/_n_//_/   |_n_,' \_,' \_,'/_/
                                <
                                 ...'

    WAFW00F - Web Application Firewall Detection Tool

    By Sandro Gauci && Wendel G. Henrique

Usage: wafw00f url1 [url2 [url3 ... ]]
example: wafw00f http://www.victim.org/

Options:
  -h, --help            show this help message and exit
  -v, --verbose         enable verbosity - multiple -v options increase
                        verbosity
  -a, --findall         Find all WAFs, do not stop testing on the first one
  -r, --disableredirect
                        Do not follow redirections given by 3xx responses
  -t TEST, --test=TEST  Test for one specific WAF
  -l, --list            List all WAFs that we are able to detect
  --xmlrpc              Switch on the XML-RPC interface instead of CUI
  --xmlrpcport=XMLRPCPORT
                        Specify an alternative port to listen on, default 8001
  -V, --version         Print out the version

~~~
