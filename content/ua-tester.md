# ua-tester command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



         _/    _/  _/_/_/_/       _/_/_/_/ _/_/_/_/ _/_/_/_/ _/_/_/_/ _/_/_/_/ _/_/_/_/
        _/    _/  _/    _/          _/    _/       _/          _/    _/       _/    _/
       _/    _/  _/_/_/_/  _/_/_/  _/    _/_/_/   _/_/_/_/    _/    _/_/_/   _/_/_/_
      _/    _/  _/    _/          _/    _/             _/    _/    _/       _/    _/
     _/_/_/_/  _/    _/          _/    _/_/_/_/ _/_/_/_/    _/    _/_/_/_/ _/      _/ [[35;40mv1.06[0m]

                                                                 _/ User-Agent Tester [35;40m↵[0m
                                                                  _/ AKA: [35;40mPurple Pimp[0m ↵
                                                                    _/ ChrisJohnRiley [35;40m↵[0m
                                                                       _/ blog.c22.cc [35;40m↵[0m



  This tool is designed to automatically check a given URL using a list of standard and non-
  standard User Agent strings provided by the user (1 per line).
  
  The results of these checks are then reported to the user for further manual analysis where 
  required. Gathered data includes Response Codes, resulting URL in the case of a 30x response,
  MD5 and length of response body, and select Server headers.

  Results: When in non-verbose mode, only values that do not match the initial reference connection
  are reported to the user. If no results are shown for a specific useragent then all results match
  the initial reference connection. If you require a full output of all checks regardless of matches
  to the reference, please use the verbose setting.
  
     Output:  [[35;40m+[0m] Added Headers, [[35;40m-[0m] Removed Headers, [[35;40m![0m] Altered Headers, [ ] No Change 

  Usage .:
            -u / --url Complete URL
            -f / --file <Path to User Agent file> / If no file is provided, -d options must be present
            -s / --single provide single user-agent string (may need to be contained within quotes)
            -d / --default Select the UA String type(s) to check. Select 1 or more of the following [35;40m↵[0m
            	           catagories. ([31;40mM[0m)obile, ([31;40mD[0m)esktop, mis([31;40mC[0m), ([31;40mT[0m)ools, ([31;40mB[0m)ots, e([31;40mX[0m)treme [[35;40m![0m])
			
	    -o / --output <Path to output file> CSV formated output (FILE WILL BE OVERWRITTEN[[31;40m![0m])
	    -v / --verbose results (Displays full headers for each check) >> Recommended
            --debug See debug messages (This isn't the switch you're looking for)


  Example .:

	    ./UATester.py -u www.example.com -f ./useragentlist.txt -v
	    ./UATester.py -u https://www.wordpress.com
	    ./UATester.py -u http://www.defaultserver.com -v --debug
	    ./UATester.py -u facebook.com -v -d MDBX
	    ./UATester.py -u https://www.google.com -s "MySpecialUserAgent"
	    ./UATester.py -u blog.c22.cc -d MC -o ./output.csv


~~~
