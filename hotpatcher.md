# hotpatcher command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: hotpatcher [options] <PID of process to patch>

Options:
-h           This help message
-V           Version number.
-v[vvvv]     Enable verbose logging. Add more 'v's for more
-N           Dry run. Do not modify anything in process
-l <.so>     Path or name of the .so file to load. Switches off execution pointer reset
-s <name>    Symbol to invoke during the dll inject. Optional.
-x <name>    Set execution pointer to symbol. Cannot be set with -s option

~~~
