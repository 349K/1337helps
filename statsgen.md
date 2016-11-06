# statsgen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: statsgen [options] passwords.txt

Type --help for more options

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -o password.masks, --output=password.masks
                        Save masks and stats to a file
  --hiderare            Hide statistics covering less than 1% of the sample
  -q, --quiet           Don't show headers.

  Password Filters:
    --minlength=8       Minimum password length
    --maxlength=8       Maximum password length
    --charset=loweralpha,numeric
                        Password charset filter (comma separated)
    --simplemask=stringdigit,allspecial
                        Password mask filter (comma separated)

~~~
