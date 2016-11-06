# mysql_setpermission command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


----------------------------------------------------------------------
                 The permission setter for MySQL.
                      version: 1.4

                 made by: Luuk de Boer <luuk@wxs.nl>
----------------------------------------------------------------------

The permission setter is a little program which can help you add users
or databases or change passwords in MySQL. Keep in mind that we don't
check permissions which already been set in MySQL. So if you can't
connect to MySQL using the permission you just added, take a look at
the permissions which have already been set in MySQL.

The permission setter first reads your .my.cnf file in your Home
directory if it exists.

Options for the permission setter:

--help		: print this help message and exit.

The options shown below are used for making the connection to the MySQL
server. Keep in mind that the permissions for the user specified via
these options must be sufficient to add users / create databases / set
passwords.

--user		: is the username to connect with.
--password	: the password of the username.
--host		: the host to connect to.
--socket	: the socket to connect to.
--port		: the port number of the host to connect to.

If you don't give a password and no password is set in your .my.cnf
file, then the permission setter will ask for a password.



~~~
