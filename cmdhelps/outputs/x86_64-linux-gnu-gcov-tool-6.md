# x86_64-linux-gnu-gcov-tool-6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: x86_64-linux-gnu-gcov-tool-6 [OPTION]... SUB_COMMAND [OPTION]...

Offline tool to handle gcda counts

  -h, --help                            Print this help, then exit
  -v, --version                         Print version number, then exit
  merge [options] <dir1> <dir2>         Merge coverage file contents
    -v, --verbose                       Verbose mode
    -o, --output <dir>                  Output directory
    -w, --weight <w1,w2>                Set weights (float point values)
  rewrite [options] <dir>               Rewrite coverage file contents
    -v, --verbose                       Verbose mode
    -o, --output <dir>                  Output directory
    -s, --scale <float or simple-frac>  Scale the profile counters
    -n, --normalize <long long>         Normalize the profile
  overlap [options] <dir1> <dir2>       Compute the overlap of two profiles
    -v, --verbose                       Verbose mode
    -h, --hotonly                       Only print info for hot objects/functions
    -f, --function                      Print function level info
    -F, --fullname                      Print full filename
    -o, --object                        Print object level info
    -t <float>, --hot_threshold <float> Set the threshold for hotness

For bug reporting instructions, please see:
<file:///usr/share/doc/gcc-6/README.Bugs>.

~~~
