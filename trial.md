# trial command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


trial [options] [[file|package|module|TestCase|testmethod]...]
Options:
  -h, --help               Display this help and exit.
  -N, --no-recurse         Don't recurse into packages
      --help-orders        Help on available test running orders
      --help-reporters     Help on available output plugins (reporters)
  -e, --rterrors           realtime errors, print out tracebacks as soon as they
                           occur
      --unclean-warnings   Turn dirty reactor errors into warnings
      --force-gc           Have Trial run gc.collect() before and after each
                           test case.
  -x, --exitfirst          Exit after the first non-successful result (cannot be
                           specified along with --jobs).
  -b, --debug              Run tests in a debugger. If that debugger is pdb,
                           will load '.pdbrc' from current directory if it
                           exists.
  -B, --debug-stacktraces  Report Deferred creation and callback stack traces
      --nopm               don't automatically jump into debugger for
                           postmorteming of exceptions
  -n, --dry-run            do everything but run the tests
      --profile            Run tests under the Python profiler
  -u, --until-failure      Repeat test until it fails
  -o, --order=             Specify what order to run test cases and methods. See
                           --help-orders for more info.
  -z, --random=            Run tests in random order using the specified seed
      --temp-directory=    Path to use as working directory for tests. [default:
                           _trial_temp]
      --reporter=          The reporter to use for this test run.  See --help-
                           reporters for more info. [default: verbose]
      --debugger=          the fully qualified name of a debugger to use if
                           --debug is passed [default: pdb]
  -l, --logfile=           log file name [default: test.log]
  -j, --jobs=              Number of local workers to run, a strictly positive
                           integer.
      --disablegc          Disable the garbage collector
      --without-module=    Fake the lack of the specified modules, separated
                           with commas.
  -r, --reactor=           Which reactor to use (see --help-reactors for a list
                           of possibilities)
      --spew               Print an insanely verbose log of everything that
                           happens.  Useful         when debugging freezes or
                           locks in complex code.
      --testmodule=        Filename to grep for test cases (-*- test-case-name).
      --version            Display Twisted version and exit.
      --coverage           Generate coverage information in the coverage file in
                           the         directory specified by the temp-directory
                           option.
      --help-reactors      Display a list of possibly available reactor names.
      --tbformat=          Specify the format to display tracebacks with. Valid
                           formats are         'plain', 'emacs', and 'cgitb'
                           which uses the nicely verbose stdlib
                           cgitb.text function
      --recursionlimit=    see sys.setrecursionlimit()

trial loads and executes a suite of unit tests, obtained from modules, packages
and files listed on the command line.


~~~
