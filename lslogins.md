# lslogins command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 lslogins [options]

Display information about known users in the system.

Options:
 -a, --acc-expiration     display info about passwords expiration
 -c, --colon-separate     display data in a format similar to /etc/passwd
 -e, --export             display in an export-able output format
 -f, --failed             display data about the users' last failed logins
 -G, --supp-groups        display information about groups
 -g, --groups=<groups>    display users belonging to a group in <groups>
 -L, --last               show info about the users' last login sessions
 -l, --logins=<logins>    display only users from <logins>
 -n, --newline            display each piece of information on a new line
     --noheadings         don't print headings
     --notruncate         don't truncate output
 -o, --output[=<list>]    define the columns to output
 -p, --pwd                display information related to login by password.
 -r, --raw                display in raw mode
 -s, --system-accs        display system accounts
     --time-format=<type> display dates in short, full or iso format
 -u, --user-accs          display user accounts
 -Z, --context            display SELinux contexts
 -z, --print0             delimit user entries with a nul character
     --wtmp-file <path>   set an alternate path for wtmp
     --btmp-file <path>   set an alternate path for btmp

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Available columns:
           USER  user name
            UID  user ID
          GECOS  full user name
        HOMEDIR  home directory
          SHELL  login shell
        NOLOGIN  log in disabled by nologin(8) or pam_nologin(8)
       PWD-LOCK  password defined, but locked
      PWD-EMPTY  password not required
       PWD-DENY  login by password disabled
          GROUP  primary group name
            GID  primary group ID
    SUPP-GROUPS  supplementary group names
      SUPP-GIDS  supplementary group IDs
     LAST-LOGIN  date of last login
       LAST-TTY  last tty used
  LAST-HOSTNAME  hostname during the last session
   FAILED-LOGIN  date of last failed login
     FAILED-TTY  where did the login fail?
         HUSHED  user's hush settings
       PWD-WARN  days user is warned of password expiration
     PWD-CHANGE  date of last password change
        PWD-MIN  number of days required between changes
        PWD-MAX  max number of days a password may remain unchanged
      PWD-EXPIR  password expiration date
        CONTEXT  the user's security context
           PROC  number of processes run by the user

For more details see lslogins(1).

~~~
