# acccheck command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

[32m
acccheck v0.2.1 - By Faiz

Description:
Attempts to connect to the IPC$ and ADMIN$ shares depending on which flags have been
chosen, and tries a combination of usernames and passwords in the hope to identify
the password to a given account via a dictionary password guessing attack.
[0m
Usage = ./acccheck [optional]

 -t [single host IP address]
 OR 
 -T [file containing target ip address(es)]

Optional:
 -p [single password]
 -P [file containing passwords]
 -u [single user]
 -U [file containing usernames]
 -v [verbose mode]

[32mExamples
Attempt the 'Administrator' account with a [BLANK] password.
	acccheck -t 10.10.10.1
Attempt all passwords in 'password.txt' against the 'Administrator' account.
	acccheck -t 10.10.10.1 -P password.txt
Attempt all password in 'password.txt' against all users in 'users.txt'.
	acccehck -t 10.10.10.1 -U users.txt -P password.txt
Attempt a single password against a single user.
	acccheck -t 10.10.10.1 -u administrator -p password
[0m
~~~
