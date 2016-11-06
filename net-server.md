# net-server command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
        net-server [base type] [net server arguments]

        net-server PreFork ipv '*'

        net-server HTTP

        net-server HTTP app foo.cgi

        net-server HTTP app foo.cgi app /=bar.cgi

        net-server HTTP port 8080 port 8443/ssl ipv '*' server_type PreFork --SSL_key_file=my.key --SSL_cert_file=my.crt access_log_file STDERR

Options:
    "base type"
        The very first argument may be a Net::Server flavor. This is given
        as shorthand for writing out server_type "ServerFlavor".
        Additionally, this allows types such as HTTP and PSGI, which are not
        true Net::Server base types, to subclass other server types via an
        additional server_type argument.

            net-server PreFork

            net-server HTTP  # becomes a HTTP server in the Fork flavor

            net-server HTTP server_type PreFork  # preforking HTTP server

    "port"
        Port to bind upon. Default is 80 if running a HTTP server as root,
        8080 if running a HTTP server as non-root, or 20203 otherwise.

        Multiple value can be given for binding to multiple ports. All of
        the methods for specifying port attributes enumerated in Net::Server
        and Net::Server::Proto are available here.

            net-server port 20201

            net-server port 20202

            net-server port 20203/IPv6

    "host"
        Host to bind to. Default is *. Will bind to an IPv4 socket if an
        IPv4 address is given. Will bind to an IPv6 socket if an IPv6
        address is given (requires installation of IO::Socket::INET6).

        If a hostname is given and "ipv" is still set to 4, an IPv4 socket
        will be created. If a hostname is given and "ipv" is set to 6, an
        IPv6 socket will be created. If a hostname is given and "ipv" is set
        to * (default), a lookup will be performed and any available IPv4 or
        IPv6 addresses will be bound. The "ipv" parameter can be set
        directly, or passed along in the port, or additionally can be passed
        as part of the hostname.

            net-server host localhost

            net-server host localhost/IPv4

    There are many more options available. Please see the Net::Server
    documentation.


~~~
