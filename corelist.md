# corelist command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
       corelist -v
       corelist [-a|-d] <ModuleName> | /<ModuleRegex>/ [<ModuleVersion>] ...
       corelist [-v <PerlVersion>] [ <ModuleName> | /<ModuleRegex>/ ] ...
       corelist [-r <PerlVersion>] ...
       corelist --feature <FeatureName> [<FeatureName>] ...
       corelist --diff PerlVersion PerlVersion
       corelist --upstream <ModuleName>

Options:
    -a  lists all versions of the given module (or the matching modules, in
        case you used a module regexp) in the perls Module::CoreList knows
        about.

            corelist -a Unicode

            Unicode was first released with perl v5.6.2
              v5.6.2     3.0.1
              v5.8.0     3.2.0
              v5.8.1     4.0.0
              v5.8.2     4.0.0
              v5.8.3     4.0.0
              v5.8.4     4.0.1
              v5.8.5     4.0.1
              v5.8.6     4.0.1
              v5.8.7     4.1.0
              v5.8.8     4.1.0
              v5.8.9     5.1.0
              v5.9.0     4.0.0
              v5.9.1     4.0.0
              v5.9.2     4.0.1
              v5.9.3     4.1.0
              v5.9.4     4.1.0
              v5.9.5     5.0.0
              v5.10.0    5.0.0
              v5.10.1    5.1.0
              v5.11.0    5.1.0
              v5.11.1    5.1.0
              v5.11.2    5.1.0
              v5.11.3    5.2.0
              v5.11.4    5.2.0
              v5.11.5    5.2.0
              v5.12.0    5.2.0
              v5.12.1    5.2.0
              v5.12.2    5.2.0
              v5.12.3    5.2.0
              v5.12.4    5.2.0
              v5.13.0    5.2.0
              v5.13.1    5.2.0
              v5.13.2    5.2.0
              v5.13.3    5.2.0
              v5.13.4    5.2.0
              v5.13.5    5.2.0
              v5.13.6    5.2.0
              v5.13.7    6.0.0
              v5.13.8    6.0.0
              v5.13.9    6.0.0
              v5.13.10   6.0.0
              v5.13.11   6.0.0
              v5.14.0    6.0.0
              v5.14.1    6.0.0
              v5.15.0    6.0.0

    -d  finds the first perl version where a module has been released by
        date, and not by version number (as is the default).

    --diff
        Given two versions of perl, this prints a human-readable table of
        all module changes between the two. The output format may change in
        the future, and is meant for *humans*, not programs. For programs,
        use the Module::CoreList API.

    -? or -help
        help! help! help! to see more help, try --man.

    -man
        all of the help

    -v  lists all of the perl release versions we got the CoreList for.

        If you pass a version argument (value of $], like 5.00503 or
        5.008008), you get a list of all the modules and their respective
        versions. (If you have the "version" module, you can also use
        new-style version numbers, like 5.8.8.)

        In module filtering context, it can be used as Perl version filter.

    -r  lists all of the perl releases and when they were released

        If you pass a perl version you get the release date for that version
        only.

    --feature, -f
        lists the first version bundle of each named feature given

    --upstream, -u
        Shows if the given module is primarily maintained in perl core or on
        CPAN and bug tracker URL.

    As a special case, if you specify the module name "Unicode", you'll get
    the version number of the Unicode Character Database bundled with the
    requested perl versions.


~~~
