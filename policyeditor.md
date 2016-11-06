# policyeditor command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


SYNOPSIS
    policyeditor
    policyeditor [-file] policy_file [-codebase] url

OPTIONS
    -codebase url     - Specifies an applet codebase URL. If the specified codebase already exists in the policy file (if any), then it will be selected when the editor opens. If it is a new codebase then it will be added and selected. Multiple URLs may also be given with a single -codebase flag by separating them with spaces. In this case, the last codebase given will be selected, and all will  be added. If this flag is given more than once, only the first is used.(Expected one or more arguments)
    -defaultfile      - Specifies that the default user-level policy file should be opened. This is the file which is normally used by IcedTea-Web to make decisions about custom policies and permissions for applets at runtime, unless configured otherwise.(No argument expected)
    -file policy_file - Specifies a policy file path to open. If exactly one argument is given, and it is not this flag, it is interpreted as a file path to open, as if this flag was given first. This flag exists mostly for compatibility with Policy Tool, but is also needed when opening a policy file and also using the -codebase flag.(Exactly one argument expected)
    -help             - Prints out information about supported command and basic usage.(No argument expected)
    -verbose          - Enable verbose output.(No argument expected)


~~~
