# jarsigner command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: jarsigner [options] jar-file alias
       jarsigner -verify [options] jar-file [alias...]

[-keystore <url>]           keystore location

[-storepass <password>]     password for keystore integrity

[-storetype <type>]         keystore type

[-keypass <password>]       password for private key (if different)

[-certchain <file>]         name of alternative certchain file

[-sigfile <file>]           name of .SF/.DSA file

[-signedjar <file>]         name of signed JAR file

[-digestalg <algorithm>]    name of digest algorithm

[-sigalg <algorithm>]       name of signature algorithm

[-verify]                   verify a signed JAR file

[-verbose[:suboptions]]     verbose output when signing/verifying.
                            suboptions can be all, grouped or summary

[-certs]                    display certificates when verbose and verifying

[-tsa <url>]                location of the Timestamping Authority

[-tsacert <alias>]          public key certificate for Timestamping Authority

[-tsapolicyid <oid>]        TSAPolicyID for Timestamping Authority

[-tsadigestalg <algorithm>] algorithm of digest data in timestamping request

[-altsigner <class>]        class name of an alternative signing mechanism

[-altsignerpath <pathlist>] location of an alternative signing mechanism

[-internalsf]               include the .SF file inside the signature block

[-sectionsonly]             don't compute hash of entire manifest

[-protected]                keystore has protected authentication path

[-providerName <name>]      provider name

[-providerClass <class>     name of cryptographic service provider's
  [-providerArg <arg>]] ... master class file and constructor argument

[-strict]                   treat warnings as errors


~~~
