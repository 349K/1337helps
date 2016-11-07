# pybuild command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: pybuild [ACTION] [BUILD SYSTEM ARGS] [DIRECTORIES] [OPTIONS]

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         turn verbose mode on
  -q, --quiet           doesn't show external command's output
  -qq, --really-quiet   be quiet
  --version             show program's version number and exit

ACTION:
  The default is to build, install and test the library using detected build
  system version by version. Selecting one of following actions, will invoke
  given action for all versions - one by one - which (contrary to the
  default action) in some build systems can overwrite previous results.

  --detect              return the name of detected build system
  --clean               clean files using auto-detected build system specific
                        methods
  --configure           invoke configure step for all requested Python
                        versions
  --build               invoke build step for all requested Python versions
  --install             invoke install step for all requested Python versions
  --test                invoke tests for auto-detected build system
  --list-systems        list available build systems and exit

BUILD SYSTEM ARGS:
  Additional arguments passed to the build system. --system=custom requires
  complete command.

  --before-clean CMD    invoked before the clean command
  --clean-args ARGS
  --after-clean CMD     invoked after the clean command
  --before-configure CMD
                        invoked before the configure command
  --configure-args ARGS
  --after-configure CMD
                        invoked after the configure command
  --before-build CMD    invoked before the build command
  --build-args ARGS
  --after-build CMD     invoked after the build command
  --before-install CMD  invoked before the install command
  --install-args ARGS
  --after-install CMD   invoked after the install command
  --before-test CMD     invoked before the test command
  --test-args ARGS
  --after-test CMD      invoked after the test command

TESTS:
  unittest's discover is used by default (if available)

  --test-nose           use nose module in --test step
  --test-pytest         use pytest module in --test step
  --test-tox            use tox in --test step

DIRECTORIES:
  -d DIR, --dir DIR     source files directory - base for other relative dirs
                        [default: CWD]
  --dest-dir DIR        destination directory [default: debian/tmp]
  --ext-dest-dir DIR    destination directory for .so files
  --ext-pattern PATTERN
                        regular expression for files that should be moved if
                        --ext-dest-dir is set [default: .so files]
  --install-dir DIR     installation directory [default: .../dist-packages]
  --name NAME           use this name to guess destination directories

LIMITATIONS:
  -s SYSTEM, --system SYSTEM
                        select a build system [default: auto-detection]
  -p VERSIONS, --pyver VERSIONS
                        build for Python VERSION. This option can be used
                        multiple times [default: all supported Python 3.X
                        versions]
  -i INTERPRETER, --interpreter INTERPRETER
                        change interpreter [default: python{version}]
  --disable ITEMS       disable action, interpreter or version

~~~
