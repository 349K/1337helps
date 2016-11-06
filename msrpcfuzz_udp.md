# msrpcfuzz_udp command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Argc=2 not 9
Usage: ./msrpcfuzz_udp target port GUID Version VersionMinor(usually 0) function_number number_of_tries max_number_of_random_items
Example: ./msrpcfuzz_udp 10.25.25.15 135 e1af8308-5d1f-11c9-91a4-08002b14a0fa 3 0 2 10 3 [OBJECT UUID]
use a while [ 1 ]; do ./msrpcfuzz ... ; done loop to make things continue nicely.
You're using MSRPCFUZZ written by Dave Aitel in November 2001
This program protected by GPL v 2.0
This program's Version = 1.0 I hope you know what you're doing. :>
Set RANDVAL=int if you don't want to use getpid()
If you're doing that, set MSRPC_DO=int as well.
Read the msrpc readme when you get a chance.

~~~
