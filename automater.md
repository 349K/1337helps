# automater command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: Automater.py [-h] [-o OUTPUT] [-b] [-f CEF] [-w WEB] [-c CSV]
                    [-d DELAY] [-s SOURCE] [--proxy PROXY] [-a USERAGENT] [-V]
                    [-r] [-v]
                    target

IP, URL, and Hash Passive Analysis tool

positional arguments:
  target                List one IP Address (CIDR or dash notation accepted),
                        URL or Hash to query or pass the filename of a file
                        containing IP Address info, URL or Hash to query each
                        separated by a newline.

optional arguments:
  -h, --help            show this help message and exit
  -o OUTPUT, --output OUTPUT
                        This option will output the results to a file.
  -b, --bot             This option will output minimized results for a bot.
  -f CEF, --cef CEF     This option will output the results to a CEF formatted
                        file.
  -w WEB, --web WEB     This option will output the results to an HTML file.
  -c CSV, --csv CSV     This option will output the results to a CSV file.
  -d DELAY, --delay DELAY
                        This will change the delay to the inputted seconds.
                        Default is 2.
  -s SOURCE, --source SOURCE
                        This option will only run the target against a
                        specific source engine to pull associated domains.
                        Options are defined in the name attribute of the site
                        element in the XML configuration file. This can be a
                        list of names separated by a semicolon.
  --proxy PROXY         This option will set a proxy to use (eg.
                        proxy.example.com:8080)
  -a USERAGENT, --useragent USERAGENT
                        This option allows the user to set the user-agent seen
                        by web servers being utilized. By default, the user-
                        agent is set to Automater/version
  -V, --vercheck        This option checks and reports versioning for
                        Automater. Checks each python module in the Automater
                        scope. Default, (no -V) is False
  -r, --refreshxml      This option refreshes the tekdefense.xml file from the
                        remote GitHub site. Default (no -r) is False.
  -v, --verbose         This option prints messages to the screen. Default (no
                        -v) is False.

~~~
