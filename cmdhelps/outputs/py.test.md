# py.test command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: py.test [options] [file_or_dir] [file_or_dir] [...]

positional arguments:
  file_or_dir

general:
  -k EXPRESSION         only run tests which match the given substring
                        expression. An expression is a python evaluatable
                        expression where all names are substring-matched
                        against test names and their parent classes. Example:
                        -k 'test_method or test_other' matches all test
                        functions and classes whose name contains
                        'test_method' or 'test_other'. Additionally keywords
                        are matched to classes and functions containing extra
                        names in their 'extra_keyword_matches' set, as well as
                        functions which have names assigned directly to them.
  -m MARKEXPR           only run tests matching given mark expression.
                        example: -m 'mark1 and not mark2'.
  --markers             show markers (builtin, plugin and per-project ones).
  -x, --exitfirst       exit instantly on first error or failed test.
  --maxfail=num         exit after first num failures or errors.
  --strict              run pytest in strict mode, warnings become errors.
  -c file               load configuration from `file` instead of trying to
                        locate one of the implicit configuration files.
  --continue-on-collection-errors
                        Force test execution even if collection errors occur.
  --fixtures, --funcargs
                        show available fixtures, sorted by plugin appearance
  --fixtures-per-test   show fixtures per test
  --import-mode={prepend,append}
                        prepend/append to sys.path when importing test
                        modules, default is to prepend.
  --pdb                 start the interactive Python debugger on errors.
  --pdbcls=modulename:classname
                        start a custom interactive Python debugger on errors.
                        For example:
                        --pdbcls=IPython.terminal.debugger:TerminalPdb
  --capture=method      per-test capturing method: one of fd|sys|no.
  -s                    shortcut for --capture=no.
  --runxfail            run tests even if they are marked xfail
  --lf, --last-failed   rerun only the tests that failed at the last run (or
                        all if none failed)
  --ff, --failed-first  run all tests but run the last failures first. This
                        may re-order tests and thus lead to repeated fixture
                        setup/teardown
  --cache-show          show cache contents, don't perform collection or tests
  --cache-clear         remove all cache contents at start of test run.

reporting:
  -v, --verbose         increase verbosity.
  -q, --quiet           decrease verbosity.
  -r chars              show extra test summary info as specified by chars
                        (f)ailed, (E)error, (s)skipped, (x)failed, (X)passed,
                        (p)passed, (P)passed with output, (a)all except pP.
                        The pytest warnings are displayed at all times except
                        when --disable-pytest-warnings is set
  --disable-pytest-warnings
                        disable warnings summary, overrides -r w flag
  -l, --showlocals      show locals in tracebacks (disabled by default).
  --tb=style            traceback print mode (auto/long/short/line/native/no).
  --full-trace          don't cut any tracebacks (default is to cut).
  --color=color         color terminal output (yes/no/auto).
  --durations=N         show N slowest setup/test durations (N=0 for all).
  --pastebin=mode       send failed|all info to bpaste.net pastebin service.
  --junit-xml=path      create junit-xml style report file at given path.
  --junit-prefix=str    prepend prefix to classnames in junit-xml output
  --result-log=path     DEPRECATED path for machine-readable result log.

collection:
  --collect-only        only collect tests, don't execute them.
  --pyargs              try to interpret all arguments as python packages.
  --ignore=path         ignore path during collection (multi-allowed).
  --confcutdir=dir      only load conftest.py's relative to specified dir.
  --noconftest          Don't load any conftest.py files.
  --keep-duplicates     Keep duplicate tests.
  --doctest-modules     run doctests in all .py modules
  --doctest-report={none,cdiff,ndiff,udiff,only_first_failure}
                        choose another output format for diffs on doctest
                        failure
  --doctest-glob=pat    doctests file matching pattern, default: test*.txt
  --doctest-ignore-import-errors
                        ignore doctest ImportErrors

test session debugging and configuration:
  --basetemp=dir        base temporary directory for this test run.
  --version             display pytest lib version and import information.
  -h, --help            show help message and configuration info
  -p name               early-load given plugin (multi-allowed). To avoid
                        loading of plugins, use the `no:` prefix, e.g.
                        `no:doctest`.
  --trace-config        trace considerations of conftest.py files.
  --debug               store internal tracing debug information in
                        'pytestdebug.log'.
  -o [OVERRIDE_INI [OVERRIDE_INI ...]], --override-ini=[OVERRIDE_INI=[OVERRIDE_INI=...]]
                        override config option, e.g. `-o xfail_strict=True`.
  --assert=MODE         Control assertion debugging tools. 'plain' performs no
                        assertion debugging. 'rewrite' (the default) rewrites
                        assert statements in test modules on import to provide
                        assert expression information.
  --setup-only          only setup fixtures, don't execute the tests.
  --setup-show          show setup fixtures while executing the tests.
  --setup-plan          show what fixtures and tests would be executed but
                        don't execute anything.


[pytest] ini-options in the next pytest.ini|tox.ini|setup.cfg file:

  markers (linelist)       markers for test functions
  norecursedirs (args)     directory patterns to avoid for recursion
  testpaths (args)         directories to search for tests when no files or dire
  usefixtures (args)       list of default fixtures to be used with this project
  python_files (args)      glob-style file patterns for Python test module disco
  python_classes (args)    prefixes or glob names for Python test class discover
  python_functions (args)  prefixes or glob names for Python test function and m
  xfail_strict (bool)      default for the strict parameter of xfail markers whe
  doctest_optionflags (args) option flags for doctests
  addopts (args)           extra command line options
  minversion (string)      minimally required pytest version

environment variables:
  PYTEST_ADDOPTS           extra command line options
  PYTEST_PLUGINS           comma-separated plugins to load during startup
  PYTEST_DEBUG             set to enable debug tracing of pytest's internals


to see available markers type: pytest --markers
to see available fixtures type: pytest --fixtures
(shown according to specified file_or_dir or current dir if not specified)

~~~
