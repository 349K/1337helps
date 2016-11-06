# purple-remote command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

This program uses D-Bus to communicate with purple.

Usage:

    /usr/bin/purple-remote "command1" "command2" ...

Each command is of one of the three types:

    [protocol:]commandname?param1=value1&param2=value2&...
    FunctionName?param1=value1&param2=value2&...
    FunctionName(value1,value2,...)

The second and third form are provided for completeness but their use
is not recommended; use purple-send or purple-send-async instead.  The
second form uses introspection to find out the parameter names and
their types, therefore it is rather slow.

Examples of commands:

    jabber:goim?screenname=testone@localhost&message=hi
    jabber:gochat?room=TestRoom&server=conference.localhost
    jabber:getinfo?screenname=testone@localhost
    jabber:addbuddy?screenname=my friend

    setstatus?status=away&message=don't disturb
    getstatus
    getstatusmessage
    quit

    PurpleAccountsFindConnected?name=&protocol=prpl-jabber
    PurpleAccountsFindConnected(,prpl-jabber)


~~~
