# rearj command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


REARJ 2.43.02, Copyright (c) 1999-2004, ARJ Software Russia. [03 Jun 2016]
All rights reserved. Archive to ARJ conversion utility
Usage:  REARJ [switch options] <!listfile(s), filespec(s) or wildname(s)>
  Switch options: (can be placed before or after filespecs)
  /+         ignore REARJ_SW variable
  /a[suffix] convert archives within archives ("*" for all formats)
  /bcommand  execute DOS command before extracting files
  /ccommand  execute DOS command on extracted files before counting them
  /d         delete original archives
  /e         no error switch
  /f         convert diskette archives
  /g         skip creation of output archive
  /i[name]   check integrity of REARJ.EXE
  /j         skip if output archive size is larger than the original
  /k         skip archive timestamping
  /l[name]   write append log file (default name is REARJ.LOG)
  /m[date]   select archives before date in YYMMDDHHMMSS format
  /n[date]   select archives on or after date in YYMMDDHHMMSS format
  /o         allow overwrite of existing target archive
  /p         ignore long filenames under Windows 95
  /q         query for each archive to convert
  /r         recurse through subdirectories
  /s         skip verify of file count and total size
  /tsuffix   create suffix type archives
  /u[bak]    allow update of archive with backup (default is BAK)
  /v         execute configured command on extracted files
  /wdir      assign work directory
  /x[!]file  exclude by filename, wildname, or listfile
  /y[text]   delete output archive and write text to log (testing mode)
  /z         simulate operation
Example:  REARJ *.* /r /d    Convert all archives to ARJ format, searching
                             all subdirectories, deleting original archives
Set REARJ environment variable: SET REARJ_SW=/l /we:\temp
REARJ log error codes:
 1 = File not found
 2 = File is not a configured archive type
 3 = Target archive already exists
 4 = Not enough disk space
 5 = User skipped or user did not select update option
 6 = UNPACK command error
 7 = PACK command error
 8 = Target cannot support directories
 9 = Wrong file count
10 = Wrong total size
11 = Internal archive REARJ error
12 = Rename archive error
13 = Invoked /v command error (found a virus?)
14 = Output archive is larger

~~~
