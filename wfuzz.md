# wfuzz command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

********************************************************
* Wfuzz 2.1.3 - The Web Bruteforcer                      *
*                                                      *
* Version up to 1.4c coded by:                         *
* Christian Martorella (cmartorella@edge-security.com) *
* Carlos del ojo (deepbit@gmail.com)                   *
*                                                      *
* Version 1.4d to 2.1.3 coded by:                        *
* Xavier Mendez (xmendez@edge-security.com)            *
********************************************************

Usage: ./wfuzz.py [options] -z payload,params <url>

Options:
-h/--help		    : This help
--version		    : Wfuzz version details
-e <type>		    : List of available encoders/payloads/iterators/printers/scripts

-c			    : Output with colors
-v			    : Verbose information. Alias for -o verbose
-o printer		    : Format output using the specified printer (default printer if omitted).
--interact		    : (beta) If selected,all key presses are captured. This allows you to interact with the program.

-p addr			    : Use Proxy in format ip:port:type or ip:port:type-...-ip:port:type for using various proxies.
			      Where type could be SOCKS4,SOCKS5 or HTTP if omitted.

-t N			    : Specify the number of concurrent connections (10 default)
-s N			    : Specify time delay between requests (0 default)
-R depth		    : Recursive path discovery being depth the maximum recursion level.
-I			    : Use HTTP HEAD method (No HTML body responses). 
--follow		    : Follow HTTP redirections
-Z			    : Scan mode (Connection errors will be ignored).

-A			    : Alias for --script=default -v -c
--script=		    : Equivalent to --script=default
--script=<plugins>	    : Runs script's scan. <plugins> is a comma separated list of plugin-files or plugin-categories
--script-help=<plugins>	    : Show help about scripts.
--script-args n1=v1,...     : Provide arguments to scripts. ie. --script-args grep.regex="<A href=\"(.*?)\">"

-m iterator		    : Specify an iterator for combining payloads (product by default)
-z payload		    : Specify a payload for each FUZZ keyword used in the form of type,parameters,encoder.
			      A list of encoders can be used, ie. md5-sha1. Encoders can be chained, ie. md5@sha1.
			      Encoders category can be used. ie. url
-w wordlist		    : Specify a wordlist file (alias for -z file,wordlist).
-V alltype		    : All parameters bruteforcing (allvars and allpost). No need for FUZZ keyword.
-X			    : Payload within HTTP methods (ex: "FUZZ HTTP/1.0"). No need for FUZZ keyword.

-b cookie		    : Specify a cookie for the requests
-d postdata 		    : Use post data (ex: "id=FUZZ&catalogue=1")
-H headers  		    : Use headers (ex:"Host:www.mysite.com,Cookie:id=1312321&user=FUZZ")
--basic/ntlm/digest auth    : in format "user:pass" or "FUZZ:FUZZ" or "domain\FUZ2Z:FUZZ"

--hc/hl/hw/hh N[,N]+	    : Hide responses with the specified code/lines/words/chars (Use BBB for taking values from baseline)
--sc/sl/sw/sh N[,N]+	    : Show responses with the specified code/lines/words/chars (Use BBB for taking values from baseline)
--ss/hs regex		    : Show/Hide responses with the specified regex within the content
--filter <filter>	    : Filter responses using the specified expression (Use BBB for taking values from baseline)
			      It should be composed of: c,l,w,h/and,or/=,<,>,!=,<=,>=

Keyword: FUZZ, ..., FUZnZ  wherever you put these keywords wfuzz will replace them with the values of the specified payload. 
Baseline: FUZZ{baseline_value} FUZZ will be replaced by baseline_value. It will be the first request performed and could be used as a base for filtering.

Examples: - wfuzz.py -c -z file,users.txt -z file,pass.txt --sc 200 http://www.site.com/log.asp?user=FUZZ&pass=FUZ2Z
	  - wfuzz.py -c -z range,1-10 --hc=BBB http://www.site.com/FUZZ{something not there}
	  - wfuzz.py --script=robots -z list,robots.txt http://www.webscantest.com/FUZZ

	   More examples in the README.

~~~
