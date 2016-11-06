# itweb-settings command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


SYNOPSIS
    itweb-settings
    itweb-settings command arguments

DESCRIPTION
    itweb-settings is a command line and a GUI program to modify and edit settings used by the IcedTea-Web implementation of javaws and the browser plugin.
    
    If executed without any arguments, it starts up a GUI. Otherwise, it tries to do what is specified in the argument.
    
    The command-line allows quickly searching, making a copy of and modifying specific settings without having to hunt through a UI.

DESCRIPTION
    -check name     - Checks that all the current settings have valid values.(No argument expected)
    -get name       - Shows the value of the specified settings.(Expected one or more arguments)
    -headless       - Disables download window, other UIs.(No argument expected)
    -help           - Prints out information about supported command and basic usage. Can also take an parameter, and then it prints detailed help for this command.(No argument expected)
    -info name      - Shows additional information about the named settings. Includes a description, the current value, the possible values, and the source of the setting.(Expected one or more arguments)
    -list           - Shows a list of all the IcedTea-Web settings and their current values.(No argument expected)
    -reset name     - Resets the specified settings to their original value.(Expected one or more arguments)
    -reset all      - Resets all settings to their original values.(No argument expected)
    -set name value - Sets the settings to the new value specified, if it is an appropriate value.(Expected even number of arguments with param=value as valid argument)
    -verbose        - Enable verbose output.(No argument expected)


~~~
