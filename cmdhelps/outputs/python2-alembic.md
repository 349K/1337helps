# python2-alembic command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: python2-alembic [-h] [-c CONFIG] [-n NAME] [-x X] [--raiseerr]
                       {branches,current,downgrade,edit,heads,history,init,list_templates,merge,revision,show,stamp,upgrade}
                       ...

positional arguments:
  {branches,current,downgrade,edit,heads,history,init,list_templates,merge,revision,show,stamp,upgrade}
    branches            Show current branch points
    current             Display the current revision for a database.
    downgrade           Revert to a previous version.
    edit                Edit revision script(s) using $EDITOR
    heads               Show current available heads in the script directory
    history             List changeset scripts in chronological order.
    init                Initialize a new scripts directory.
    list_templates      List available templates
    merge               Merge two revisions together. Creates a new migration
                        file. .. versionadded:: 0.7.0 .. seealso::
                        :ref:`branches`
    revision            Create a new revision file.
    show                Show the revision(s) denoted by the given symbol.
    stamp               'stamp' the revision table with the given revision;
                        don't run any migrations.
    upgrade             Upgrade to a later version.

optional arguments:
  -h, --help            show this help message and exit
  -c CONFIG, --config CONFIG
                        Alternate config file
  -n NAME, --name NAME  Name of section in .ini file to use for Alembic config
  -x X                  Additional arguments consumed by custom env.py
                        scripts, e.g. -x setting1=somesetting -x
                        setting2=somesetting
  --raiseerr            Raise a full stack trace on error

~~~
