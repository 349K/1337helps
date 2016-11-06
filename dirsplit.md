# dirsplit command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


dirsplit [options] [advanced options] < directory >

 -H|--longhelp Show the long help message with more advanced options
 -n|--no-act   Only print the commands, no action (implies -v)
 -s|--size     NUMBER - Size of the medium (default: 4488M)
 -e|--expmode  NUMBER - directory exploration mode (recommended, see long help)
 -m|--move     Move files to target dirs (default: create mkisofs catalogs)
 -p|--prefix   STRING - first part of catalog/directory name (default: vol_)
 -h|--help     Show this option summary
 -v|--verbose  More verbosity
                   
The complete help can be displayed with the --longhelp (-H) option.
The default mode is creating file catalogs useable with:
    mkisofs -D -r --joliet-long -graft-points -path-list CATALOG

Example:
dirsplit -m -s 700M -e2 random_data_to_backup/

~~~
