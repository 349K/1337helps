# futility_s command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: futility [options] COMMAND [args...]

This is the unified firmware utility, which will eventually replace
most of the distinct verified boot tools formerly produced by the
vboot_reference package.

When symlinked under the name of one of those previous tools, it should
fully implement the original behavior. It can also be invoked directly
as futility, followed by the original name as the first argument.

Global options:

  --vb1        Use only vboot v1.0 binary formats
  --vb21       Use only vboot v2.1 binary formats
  --debug      Be noisy about what's going on

The following commands are built-in:

  dump_fmap            Display FMAP contents from a firmware image
  gbb_utility          Manipulate the Google Binary Block (GBB)
  help                 Show a bit of help (you're looking at it)
  version              Show the futility source revision and build date

Use "futility help COMMAND" for more information.


~~~
