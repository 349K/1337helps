# cewl command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

CeWL 5.2 (Some Chaos) Robin Wood (robin@digi.ninja) (https://digi.ninja/)
Usage: cewl [OPTION] ... URL
    --help, -h: show help
    --keep, -k: keep the downloaded file
    --depth x, -d x: depth to spider to, default 2
    --min_word_length, -m: minimum word length, default 3
    --offsite, -o: let the spider visit other sites
    --write, -w file: write the output to the file
    --ua, -u user-agent: user agent to send
    --no-words, -n: don't output the wordlist
    --meta, -a include meta data
    --meta_file file: output file for meta data
    --email, -e include email addresses
    --email_file file: output file for email addresses
    --meta-temp-dir directory: the temporary directory used by exiftool when parsing files, default /tmp
    --count, -c: show the count for each word found

    Authentication
    --auth_type: digest or basic
    --auth_user: authentication username
    --auth_pass: authentication password

    Proxy Support
    --proxy_host: proxy host
    --proxy_port: proxy port, default 8080
    --proxy_username: username for proxy, if required
    --proxy_password: password for proxy, if required

    --verbose, -v: verbose

    URL: The site to spider.


~~~
