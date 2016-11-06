# wsgen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

unrecognized parameter --help


Usage: WSGEN [options] <SEI>

where [options] include:
  -classpath <path>          specify where to find input class files and wsgen extensions
  -cp <path>                 specify where to find input class files and wsgen extensions
  -d <directory>             specify where to place generated output files
  -encoding <encoding>       specify character encoding used by source files
  -extension                 allow vendor extensions - functionality not specified
                             by the specification.  Use of extensions may
                             result in applications that are not portable or
                             may not interoperate with other implementations
  -help                      display help
  -J<javacOption>            pass this option to javac
  -keep                      keep generated files
  -r <directory>             resource destination directory, specify where to
                             place resouce files such as WSDLs
  -s <directory>             specify where to place generated source files
  -verbose                   output messages about what the compiler is doing
  -version                   print version information
  -fullversion               print full version information
  -wsdl[:protocol]           generate a WSDL file. The protocol is optional.
                             Valid protocols are [soap1.1, Xsoap1.2],
                             the default is soap1.1.
                             The non standard protocols [Xsoap1.2]
                             can only be used in conjunction with the
                             -extension option.
  -inlineSchemas             inline schemas in the generated wsdl. Must be
                             used in conjunction with the -wsdl option.
  -servicename <name>        specify the Service name to use in the generated WSDL
                             Used in conjunction with the -wsdl option.
  -portname <name>           specify the Port name to use in the generated WSDL
                             Used in conjunction with the -wsdl option.
  -x <file>                  specify External Web Service Metadata xml descriptor

Extensions:
  -Xnocompile                do not compile generated Java files

Examples:
  wsgen -cp . example.Stock
  wsgen -cp . example.Stock -wsdl -servicename {http://mynamespace}MyService


~~~
