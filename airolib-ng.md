# airolib-ng command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


  Airolib-ng 1.2 rc4 - (C) 2007, 2008, 2009 ebfe
  http://www.aircrack-ng.org

  Usage: airolib-ng <database> <operation> [options]

  Operations:

       --stats        : Output information about the database.
       --sql <sql>    : Execute specified SQL statement.
       --clean [all]  : Clean the database from old junk. 'all' will also 
                        reduce filesize if possible and run an integrity check.
       --batch        : Start batch-processing all combinations of ESSIDs
                        and passwords.
       --verify [all] : Verify a set of randomly chosen PMKs.
                        If 'all' is given, all invalid PMK will be deleted.

       --import [essid|passwd] <file>   :
                        Import a text file as a list of ESSIDs or passwords.
       --import cowpatty <file>         :
                        Import a cowpatty file.

       --export cowpatty <essid> <file> :
                        Export to a cowpatty file.


~~~
