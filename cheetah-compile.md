# cheetah-compile command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: cheetah-compile [options]

Options:
  -h, --help            show this help message and exit
  --idir=IDIR           Input directory (defaults to current directory)
  --odir=ODIR           Output directory (defaults to current directory)
  --iext=IEXT           File input extension (defaults: compile: .tmpl, fill:
                        .tmpl)
  --oext=OEXT           File output extension (defaults: compile: .py, fill:
                        .html)
  -R                    Recurse through subdirectories looking for input files
  -p, --stdout          Send output to stdout instead of writing to a file
  --quiet               Do not print informational messages to stdout
  --debug               Print diagnostic/debug information to stderr
  --env                 Pass the environment into the search list
  --pickle=PICKLE       Unpickle FILE and pass it through in the search list
  --flat                Do not build destination subdirectories
  --nobackup            Do not make backup files when generating new ones
  --settings=COMPILERSETTINGSSTRING
                        String of compiler settings to pass through, e.g.
                        --settings="useNameMapper=False,useFilters=False"
  --print-settings      Print out the list of available compiler settings
  --templateAPIClass=TEMPLATECLASSNAME
                        Name of a subclass of Cheetah.Template.Template to use
                        for compilation, e.g. MyTemplateClass
  --parallel=PARALLEL   Compile/fill templates in parallel, e.g. --parallel=4
  --shbang=SHBANG       Specify the shbang to place at the top of compiled
                        templates, e.g. --shbang="#!/usr/bin/python2.6"

~~~
