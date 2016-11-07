# reportbug command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: reportbug [options] <package | filename>

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -c, --no-config-files
                        do not include conffiles in report
  -C CLASS, --class=CLASS
                        specify report class for GNATS BTSes
  -d, --debug           send report only to yourself
  --test                operate in test mode (maintainer use only)
  -e EDITOR, --editor=EDITOR
                        specify an editor for your report
  -f SEARCHFOR, --filename=SEARCHFOR
                        report the bug against the package containing the
                        specified file
  --from-buildd=BUILDD_FORMAT
                        parse information from buildd format: $source_$version
  --path                only search the path with -f
  -g, --gnupg, --gpg    sign report with GNU Privacy Guard (GnuPG/gpg)
  -G, --gnus            send the report using Gnus
  --pgp                 sign report with Pretty Good Privacy (PGP)
  -K KEYID, --keyid=KEYID
                        key ID to use for PGP/GnuPG signatures
  -H HEADERS, --header=HEADERS
                        add a custom RFC2822 header to your report
  -P PSEUDOS, --pseudo-header=PSEUDOS
                        add a custom pseudo-header to your report
  --license             show copyright and license information
  -m, --maintonly       send the report to the maintainer only
  -M, --mutt            send the report using mutt
  --mirror=MIRRORS      add a BTS mirror
  -n, --mh, --nmh       send the report using mh/nmh
  -N, --bugnumber       specify a bug number to look for
  --mua=MUA             send the report using the specified mail user agent
  --mta=MTA             send the report using the specified mail transport
                        agent
  --list-cc=LISTCC      send a copy to the specified address
  -p, --print           output the report to standard output only
  --report-quiet        file report without any mail to the maintainer or
                        tracking lists
  -q, --quiet           reduce the verbosity of the output
  -s SUBJECT, --subject=SUBJECT
                        the subject for your report
  -x, --no-cc           do not send a copy of the report to yourself
  -z, --no-compress     do not strip blank lines and comments from config
                        files
  -o OUTFILE, --output=OUTFILE
                        output the report to the specified file (both mail
                        headers and body)
  -O, --offline         disable all external queries
  -i INCLUDE, --include=INCLUDE
                        include the specified file in the report
  -A ATTACHMENTS, --attach=ATTACHMENTS
                        attach the specified file to the report
  -b, --no-query-bts    do not query the BTS for reports
  --query-bts           query the BTS for reports
  -T TAGS, --tag=TAGS   add the specified tag to the report
  --http_proxy=HTTP_PROXY, --proxy=HTTP_PROXY
                        use this proxy for HTTP accesses
  --email=EMAIL         specify originating email address
  --realname=REALNAME   specify real name for your report
  --smtphost=SMTPHOST   specify SMTP server for mailing
  --tls                 use TLS to talk to SMTP servers
  --source, --src       report the bug against the source package
  --smtpuser=SMTPUSER   username to use for SMTP
  --smtppasswd=SMTPPASSWD
                        password to use for SMTP
  --replyto=REPLYTO, --reply-to=REPLYTO
                        specify Reply-To address for your report
  --query-source        query on source packages, not binary packages
  --no-query-source     query on binary packages only
  --security-team       send the report only to the security team, if
                        tag=security
  --no-security-team    do not send the report only to the security team, if
                        tag=security
  --debconf             include debconf settings in your report
  --no-debconf          exclude debconf settings from your report
  -j JUSTIFICATION, --justification=JUSTIFICATION
                        include justification for the severity of your report
  -V PKGVERSION, --package-version=PKGVERSION
                        specify the version number for the package
  -u INTERFACE, --interface=INTERFACE, --ui=INTERFACE
                        choose which user interface to use
  -Q, --query-only      only query the BTS
  -t TYPE, --type=TYPE  choose the type of report to file
  -B BTS, --bts=BTS     choose BTS to file the report with
  -S SEVERITY, --severity=SEVERITY
                        identify the severity of the report
  --template            output a template report only
  --configure           reconfigure reportbug for this user
  --check-available     check for new releases on various sites
  --no-check-available  do not check for new releases
  --mode=MODE           choose the operating mode for reportbug
  -v, --verify          verify integrity of installed package using debsums
  --no-verify           do not verify package installation
  -k, --kudos           send appreciative email to the maintainer, rather than
                        filing a bug report
  --body=BODY           specify the body for the report as a string
  --body-file=BODYFILE, --bodyfile=BODYFILE
                        use the specified file as the body of the report
  -I, --no-check-installed
                        don't check whether the package is installed
  --check-installed     check whether the specified package is installed when
                        filing a report (default)
  --exit-prompt         prompt before exiting
  --paranoid            show contents of message before sending
  --no-paranoid         don't show contents of message before sending
                        (default)
  --no-bug-script       don't execute the bug script (if present)
  --draftpath=DRAFTPATH
                        Save the draft in this directory
  --timeout=TIMEOUT     Specify the network timeout, in seconds [default: 60]
  --no-cc-menu          don't show additional CC menu
  --no-tags-menu        don't show tags menu
  --mbox-reader-cmd=MBOX_READER_CMD
                        Specify the program to open the reports mbox.
  --max-attachment-size=MAX_ATTACHMENT_SIZE
                        Specify the maximum size in byte for an attachment
                        [default: 10485760].
  --latest-first        Order bugs to show the latest first
  --envelope-from=ENVELOPEFROM
                        Specify the Envelope From (Return-path) address used
                        to send the bug report

~~~
