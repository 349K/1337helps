# javaws command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


SYNOPSIS
    javaws [-run-options] jnlp file
    javaws [-control-options]

OPTIONS
    When specifying options, the name of the jnlp file can be after the command, the -jnlp option, an option with no arguments, or after an argument with an option that takes one argument. A html file that launches a jnlp can be specified after the -html option.
    The jnlp-file can either be a url or a local path.
    The JNLP file should only be specified once, whether as a main argument, after -jnlp or through an html file.
    Control options:
    -about               - Shows a sample application.(No argument expected)
    -help                - Prints out information about supported command and basic usage.(No argument expected)
    -license             - Display the GPL license and exit.(No argument expected)
    -viewer              - Shows the trusted certificate viewer.(No argument expected)
    -Xclearcache         - Clean the JNLP application cache.(No argument expected)
    Run options:
    -allowredirect       - Follows HTTP redirects.(No argument expected)
    -arg arg             - Adds an application argument before launching.(Expected one or more arguments)
    -headless            - Disables download window, other UIs.(No argument expected)
    -html                - Location of HTML file to launch (url or file). You can use parameter ALL  or numbers (like 1 2 5) to select applets on page. However experimental, this switch should keep you still in safety.(Expected one or more arguments)
    -jnlp                - Location of JNLP file to launch (url or file).(Exactly one argument expected)
    -nosecurity          - Disables the secure runtime environment.(No argument expected)
    -noupdate            - Disables checking for updates.(No argument expected)
    -param name=value    - Adds an applet parameter before launching.(Expected one or more arguments)
    -property name=value - Sets a system property before launching.(Expected one or more arguments)
    -strict              - Enables strict checking of JNLP file format.(No argument expected)
    -update seconds      - Check for updates.(Exactly one argument expected)
    -verbose             - Enable verbose output.(No argument expected)
    -version             - Print the IcedTea-Web version and exit.(No argument expected)
    -Xignoreheaders      - Skip jar header verification.(No argument expected)
    -xml                 - Uses a strict XML parser to parse the JNLP file.(No argument expected)
    -Xnofork             - Do not create another JVM.(No argument expected)
    -Xoffline            - Prevent ITW network connection. Only cache will be used. Application can still connect.(No argument expected)
    -Xtrustnone          - Instead of asking user, will foretold all answers as no.(No argument expected)


~~~
