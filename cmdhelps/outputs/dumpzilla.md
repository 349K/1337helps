# dumpzilla command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Version: 15/03/2013

Usage: python dumpzilla.py browser_profile_directory [Options]

Options:

 --All (Shows everything but the DOM data. Doesn't extract thumbnails or HTML 5 offline)
 --Cookies [-showdom -domain <string> -name <string> -hostcookie <string> -access <date> -create <date> -secure <0/1> -httponly <0/1> -range_last -range_create <start> <end>]
 --Permissions [-host <string>]
 --Downloads [-range <start> <end>]
 --Forms	[-value <string> -range_forms <start> <end>]
 --History [-url <string> -title <string> -date <date> -range_history <start> <end> -frequency]
 --Bookmarks [-range_bookmarks <start> <end>]
 --Cacheoffline [-range_cacheoff <start> <end> -extract <directory>]
 --Thumbnails [-extract_thumb <directory>]
 --Range <start date> <end date>
 --Addons
 --Passwords (Decode only in Unix)
 --Certoverride
 --Session
 --Watch [-text <string>] (Shows in daemon mode the URLs and text form in real time. -text' Option allow filter,  support all grep Wildcards. Exit: Ctrl + C. only Unix).

Wildcards: '%'  Any string of any length (Including zero length)
           '_'  Single character
	   '\'  Escape character

Date syntax: YYYY-MM-DD HH:MM:SS

Win profile: 'C:\Documents and Settings\xx\Application Data\Mozilla\Firefox\Profiles\xxxx.default'
Unix profile: '/home/xx/.mozilla/seamonkey/xxxx.default/'


~~~
