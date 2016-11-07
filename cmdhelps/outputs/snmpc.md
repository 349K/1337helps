# snmpc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: snmpc [options] MIB.mib|MIB.bin
Compile a MIB (.mib -> .bin) or generate an erlang header 
file from a compiled MIB file (.bin -> .hrl)
Options:
   --help                   - Prints this info.
   --version                - Prints compiler version.
   --verbosity <verbosity>  - Print debug info.
                              verbosity = trace | debug | log | info | silence
                              Defaults to silence.
   --warnings | --W         - Print warning messages.
   --o <output dir>         - The output dir.
                              Defaults to current working dir.
   --i <include dir>        - Add this dir to the list of dirs that will be
                              searched for imported (compiled) MIB files.
                              The current workin dir will always be included. 
   --il <include_lib dir>   - Add this dir to the list of dirs that will be
                              searched for imported (compiled) MIB files.
                              It assumes that the first element in the dir 
                              name correspond to an OTP application. 
                              For example snmp/mibs/ 
                              The current workin dir and the 
                              <snmp-home>/priv/mibs 
                              are always listed last the includ path. 
   --db <DB>                - Database to used for the default instrumentation.
                              Defaults to volatile.
   --sgc                    - This option (skip group check), if present, 
                              disables the "group check" of the mib compiler. 
                              That is, should the OBJECT-GROUP and the 
                              NOTIFICATION-GROUP macro(s) be checked for 
                              correctness or not. 
                              By default the check is done. 
   --dep                    - Keep deprecated definition(s).
                              If not specified the compiler will ignore
                              deprecated definitions.
   --desc                   - The DESCRIPTION field will be included.
   --ref                    - The REFERENCE field will be included.
   --imp                    - The IMPORTS field will be included.
   --mi                     - The MODULE-IDENTITY field will be included.
   --mc                     - The MODULE-COMPLIANCE field will be included.
   --ac                     - The AGENT-CAPABILITIES field will be included.
   --mod <module>           - The module which implements all the 
                              instrumentation functions. 
                              The name of all instrumentation functions must
                              be the same as the corresponding managed object
                              it implements.
   --nd                     - The default instrumentation functions will *not* 
                              be used if a managed object have no 
                              instrumentation function. Instead this will be 
                              reported as an error, and the compilation aborts. 
   --rrnac                  - This option, if present, specifies that the row 
                              name assign check shall not be done strictly 
                              according to the SMI (which allows only the 
                              value 1). With this option, all values greater 
                              than zero is allowed (>= 1). 
                              This means that the error will be converted to 
                              a warning. 
                              By default it is not included, but if this 
                              option is present it will be. 
   --wae | --Werror         - Warnings as errors. 
                              Indicates that warnings shall be treated as 
                              errors. 
   

~~~
