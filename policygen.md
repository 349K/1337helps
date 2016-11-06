# policygen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: policygen [options]

Type --help for more options

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -o masks.hcmask, --outputmasks=masks.hcmask
                        Save masks to a file
  --pps=1000000000      Passwords per Second
  --showmasks           Show matching masks
  --noncompliant        Generate masks for noncompliant passwords
  -q, --quiet           Don't show headers.

  Password Policy:
    Define the minimum (or maximum) password strength policy that you
    would like to test

    --minlength=8       Minimum password length
    --maxlength=8       Maximum password length
    --mindigit=1        Minimum number of digits
    --minlower=1        Minimum number of lower-case characters
    --minupper=1        Minimum number of upper-case characters
    --minspecial=1      Minimum number of special characters
    --maxdigit=3        Maximum number of digits
    --maxlower=3        Maximum number of lower-case characters
    --maxupper=3        Maximum number of upper-case characters
    --maxspecial=3      Maximum number of special characters

~~~
