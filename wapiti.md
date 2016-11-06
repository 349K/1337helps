# wapiti command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Wapiti-2.3.0 (wapiti.sourceforge.net)
Wapiti-2.3.0 - Web application vulnerability scanner 
 
 Usage: python wapiti.py http://server.com/base/url/ [options] 
 
 Supported options are: 
 -s <url> 
 --start <url> 
 	To specify an url to start with. This option can be called several times.
 	Wapiti will browse these links to find more URLs even if the specified link is not in the scope.
 
 -x <url> 
 --exclude <url> 
 	To exclude an URL from the scan (eg: logout URLs). This option can be called several times to specify several URLs.
 	Wildcards (*) can be used in URLs for basic regex.
 	Example : -x http://server/base/?page=*&module=test
 	or -x http://server/base/admin/* to exclude a directory.
 
 -p <url_proxy> 
 --proxy <url_proxy> 
 	To specify a proxy. Currently supported proxies are HTTP and HTTPS.
 	This option can be called twice to specify the HTTP and the HTTPS proxy.
 	Example: -p http://proxy:port/
 
 -c <cookie_file> 
 --cookie <cookie_file> 
 	To import cookies to use for the scan. The cookie file must be in JSON format.
 	Cookies can be grabbed using the cookie.py and getcookie.py utilities (net directory).
 
 -t <timeout> 
 --timeout <timeout> 
 	To set the timeout (maximum time in seconds to wait for the server to send a response).
 
 -a <login%password> 
 --auth <login%password> 
 	Set credentials for HTTP authentication.
 
 --auth-method <method>
 	If the server requires an authentication, set the authentication method to use.
 	Currently supported methods are (some requires additional modules to install):
 		+ basic
 		+ digest
 		+ kerberos
 		+ ntlm
 
 -r <parameter_name> 
 --remove <parameter_name> 
 	Remove a parameter (name and value) from URLs.
 
 -n <limit> 
 --nice <limit> 
 	Define a limit of URLs to browse with the same pattern (ie, the maximum number of unique values for the same parameter).
 	Use this option to prevent endless loops during scan. Limit must be greater than 0.
 
 -m <module_options>
 --module <module_options>
 	Set the modules (and HTTP methods for each module) to use for attacks.
 	Prefix a module name with a dash to deactivate the related module.
 	To only browse the target (without sending any payloads), deactivate every module with -m "-all".
 	If you don't specify the HTTP methods, GET and POST will be used.
 	Example: -m "-all,xss:get,exec:post"
 
 -u 
 --color 
 	Use colors to highlight vulnerabilities and anomalies in output. 
 
 -v <level> 
 --verbose <level> 
 	Set the verbosity level. 
 	0: quiet (default), 1: print each URL, 2: print every attack. 
 
 -b <scope>
 --scope <scope>
 	Set the scope of the scan:
 		+ page: to analyse only the page given as the root URL.
 		+ folder: to analyse all the URLs under the root URL passed to Wapiti (default).
 		+ domain: to analyse all the links to the pages which are in the same domain as the URL passed to Wapiti.
 
 -f <type_file> 
 --format <type_file> 
 	Set the format type for the report. 
 	json: Report in JSON format 
 	html: Report in HTML format (default)
 	openvas: Report in OpenVAS XML format 
 	txt: Report in plain text (UTF-8) 
 	vulneranet: Report in VulneraNET (XML based) format 
 	xml: Report in XML format 
 
 -o <output> 
 --output <output_file> 
 	Set the name of the report file. 
 	If the selected report format is 'html', this parameter will be used as a directory name.
 
 -i <file>
 --continue <file>
 	This parameter indicates to Wapiti to resume the previous scan saved in the
specified XML status file.
 	The file name is optional, if not specified, Wapiti takes the default file from the "scans" folder.
 
 -k <file>
 --attack <file>
 	This parameter indicates to Wapiti to resume the attacks without scanning the website again, loading the scan status from the specified file.
 	The file name is optional, if it is not specified, Wapiti takes the default file from the "scans" folder.
 
 --verify-ssl <0|1>
 	This parameter indicates whether Wapiti must check SSL certificates.
 	Default is to verify certificates
 
 -h 
 --help 
 	To print this usage message
 

~~~
