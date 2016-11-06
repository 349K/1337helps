# pg_virtualenv command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


pg_virtualenv: Create throw-away PostgreSQL environment for regression tests
Syntax: /usr/bin/pg_virtualenv [options] [command]
    -a                use all installed server versions
    -v 'version ...'  list of PostgreSQL versions to run [default: latest]
    -c 'options'      extra options to pass to pg_createcluster
    -i 'initdb opts'  extra initdb options to pass to pg_createcluster
    -o 'guc=value'    postgresql.conf options to pass to pg_createcluster
    -s                open a shell when command fails
    -t                use a temporary cluster directory even as root

~~~
