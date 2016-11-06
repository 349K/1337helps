# besside-ng-crawler command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Use: besside-ng-crawler <SearchDir> <CapFileOut>
What does it do?

It recurses the SearchDir directory
Opens all files in there, searching for pcap-dumpfiles
Filters out a single beacon and all EAPOL frames from the WPA networks in there
And saves them to CapFileOut.

This tool is supposed to crawl capfiles for upload to sorbo's WPA statistic server!

~~~
