# update-leap command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

    update-leap
        Usage: $0 [options] [leapfile]

        Verifies and if necessary, updates leap-second definition file

        All arguments are optional: Default (or current value) shown: -s
        Specify the URL of the master copy to download $LEAPSRC -d Specify
        the filename on the local system $LEAPFILE -e Specify how long (in
        days) before expiration the file is to be refreshed. Note that
        larger values imply more frequent refreshes. "$PREFETCH" -f Specify
        location of ntp.conf (used to make sure leapfile directive is
        present and to default leapfile) $NTPCONF -F Force update even if
        current file is OK and not close to expiring. -r Specify number of
        times to retry on get failure $MAXTRIES -i Specify number of minutes
        between retries $INTERVAL -l Use syslog for output (Implied if
        CRONJOB is set) -L Don't use syslog for output -P Specify the syslog
        facility for logging $LOGFAC -t Name of temporary file used in
        validation $TMPFILE -q Only report errors to stdout -v Verbose
        output

        The following options are not (yet) implemented in the perl version:
        -4 Use only IPv4 -6 Use only IPv6 -c Command to restart NTP after
        installing a new file <none> - ntpd checks file daily -p 4|6 Prefer
        IPv4 or IPv6 (as specified) addresses, but use either -z Specify
        path for utilities $PATHLIST -Z Only use system path

        $0 will validate the file currently on the local system

        Ordinarily, the file is found using the "leapfile" directive in
        $NTPCONF. However, an alternate location can be specified on the
        command line.

        If the file does not exist, is not valid, has expired, or is
        expiring soon, a new copy will be downloaded. If the new copy
        validates, it is installed and NTP is (optionally) restarted.

        If the current file is acceptable, no download or restart occurs.

        -c can also be used to invoke another script to perform
        administrative functions, e.g. to copy the file to other local
        systems.

        This can be run as a cron job. As the file is rarely updated, and
        leap seconds are announced at least one month in advance (usually
        longer), it need not be run more frequently than about once every
        three weeks.

        For cron-friendly behavior, define CRONJOB=1 in the crontab.

        Version $VERSION


~~~
