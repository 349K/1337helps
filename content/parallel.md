# parallel command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:

parallel [options] [command [arguments]] < list_of_arguments
parallel [options] [command [arguments]] (::: arguments|:::: argfile(s))...
cat ... | parallel --pipe [options] [command [arguments]]

-j n            Run n jobs in parallel
-k              Keep same order
-X              Multiple arguments with context replace
--colsep regexp Split input on regexp for positional replacements
{} {.} {/} {/.} {#} {%} {= perl code =} Replacement strings
{3} {3.} {3/} {3/.} {=3 perl code =}    Positional replacement strings
With --plus:    {} = {+/}/{/} = {.}.{+.} = {+/}/{/.}.{+.} = {..}.{+..} =
                {+/}/{/..}.{+..} = {...}.{+...} = {+/}/{/...}.{+...}

-S sshlogin     Example: foo@server.example.com
--slf ..        Use ~/.parallel/sshloginfile as the list of sshlogins
--trc {}.bar    Shorthand for --transfer --return {}.bar --cleanup
--onall         Run the given command with argument on all sshlogins
--nonall        Run the given command with no arguments on all sshlogins

--pipe          Split stdin (standard input) to multiple jobs.
--recend str    Record end separator for --pipe.
--recstart str  Record start separator for --pipe.

See 'man parallel' for details

When using programs that use GNU Parallel to process data for publication please cite:

O. Tange (2011): GNU Parallel - The Command-Line Power Tool,
;login: The USENIX Magazine, February 2011:42-47.

Or you can get GNU Parallel without this requirement by paying 10000 EUR.

~~~
