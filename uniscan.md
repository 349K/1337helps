# uniscan command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

####################################
# Uniscan project                  #
# http://uniscan.sourceforge.net/  #
####################################
V. 6.3


OPTIONS:
	-h 	help
	-u 	<url> example: https://www.example.com/
	-f 	<file> list of url's
	-b 	Uniscan go to background
	-q 	Enable Directory checks
	-w 	Enable File checks
	-e 	Enable robots.txt and sitemap.xml check
	-d 	Enable Dynamic checks
	-s 	Enable Static checks
	-r 	Enable Stress checks
	-i 	<dork> Bing search
	-o 	<dork> Google search
	-g 	Web fingerprint
	-j 	Server fingerprint

usage: 
[1] perl ./uniscan.pl -u http://www.example.com/ -qweds
[2] perl ./uniscan.pl -f sites.txt -bqweds
[3] perl ./uniscan.pl -i uniscan
[4] perl ./uniscan.pl -i "ip:xxx.xxx.xxx.xxx"
[5] perl ./uniscan.pl -o "inurl:test"
[6] perl ./uniscan.pl -u https://www.example.com/ -r



~~~
