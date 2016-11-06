# glib-compile-resources command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
  glib-compile-resources [OPTION...] FILE

Compile a resource specification into a resource file.
Resource specification files have the extension .gresource.xml,
and the resource file have the extension called .gresource.

Help Options:
  -h, --help                  Show help options

Application Options:
  --version                   Show program version and exit
  --target=FILE               name of the output file
  --sourcedir=DIRECTORY       The directories where files are to be read from (default to current directory)
  --generate                  Generate output in the format selected for by the target filename extension
  --generate-header           Generate source header
  --generate-source           Generate sourcecode used to link in the resource file into your code
  --generate-dependencies     Generate dependency list
  --dependency-file=FILE      name of the dependency file to generate
  --manual-register           Don't automatically create and register resource
  --internal                  Don't export functions; declare them G_GNUC_INTERNAL
  --c-name                    C identifier name used for the generated source code


~~~
