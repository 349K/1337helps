# sudo command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

sudo - execute a command as another user

usage: sudo -h | -K | -k | -V
usage: sudo -v [-AknS] [-g group] [-h host] [-p prompt] [-u user]
usage: sudo -l [-AknS] [-g group] [-h host] [-p prompt] [-U user] [-u user] [command]
usage: sudo [-AbEHknPS] [-r role] [-t type] [-C num] [-g group] [-h host] [-p prompt] [-u user] [VAR=value] [-i|-s]
            [<command>]
usage: sudo -e [-AknS] [-r role] [-t type] [-C num] [-g group] [-h host] [-p prompt] [-u user] file ...

Options:
  -A, --askpass               use a helper program for password prompting
  -b, --background            run command in the background
  -C, --close-from=num        close all file descriptors >= num
  -E, --preserve-env          preserve user environment when running command
  -e, --edit                  edit files instead of running a command
  -g, --group=group           run command as the specified group name or ID
  -H, --set-home              set HOME variable to target user's home dir
  -h, --help                  display help message and exit
  -h, --host=host             run command on host (if supported by plugin)
  -i, --login                 run login shell as the target user; a command may also be specified
  -K, --remove-timestamp      remove timestamp file completely
  -k, --reset-timestamp       invalidate timestamp file
  -l, --list                  list user's privileges or check a specific command; use twice for longer format
  -n, --non-interactive       non-interactive mode, no prompts are used
  -P, --preserve-groups       preserve group vector instead of setting to target's
  -p, --prompt=prompt         use the specified password prompt
  -r, --role=role             create SELinux security context with specified role
  -S, --stdin                 read password from standard input
  -s, --shell                 run shell as the target user; a command may also be specified
  -t, --type=type             create SELinux security context with specified type
  -U, --other-user=user       in list mode, display privileges for user
  -u, --user=user             run command (or edit file) as specified user name or ID
  -V, --version               display version information and exit
  -v, --validate              update user's timestamp without running a command
  --                          stop processing command line arguments

~~~
