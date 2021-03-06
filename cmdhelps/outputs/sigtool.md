# sigtool command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



Clam AntiVirus: Signature Tool (sigtool)  0.99.2
       By The ClamAV Team: http://www.clamav.net/team
       (C) 2007-2015 Cisco Systems, Inc.

    --help                 -h              show help
    --version              -V              print version number and exit
    --quiet                                be quiet, output only error messages
    --debug                                enable debug messages
    --stdout                               write to stdout instead of stderr
    --hex-dump                             convert data from stdin to a hex
                                           string and print it on stdout
    --md5 [FILES]                          generate MD5 checksum from stdin
                                           or MD5 sigs for FILES
    --sha1 [FILES]                         generate SHA1 checksum from stdin
                                           or SHA1 sigs for FILES
    --sha256 [FILES]                       generate SHA256 checksum from stdin
                                           or SHA256 sigs for FILES
    --mdb [FILES]                          generate .mdb sigs
    --html-normalise=FILE                  create normalised parts of HTML file
    --ascii-normalise=FILE                 create normalised text file from ascii source
    --utf16-decode=FILE                    decode UTF16 encoded files
    --info=FILE            -i FILE         print database information
    --build=NAME [cvd] -b NAME             build a CVD file
    --max-bad-sigs=NUMBER                  Maximum number of mismatched signatures
                                           when building a CVD. Default: 3000
    --flevel=FLEVEL                        Specify a custom flevel.
                                           Default: 82
    --cvd-version=NUMBER                   Specify the version number to use for
                                           the build. Default is to use the value+1
                                           from the current CVD in --datadir.
                                           If no datafile is found the default
                                           behaviour is to prompt for a version
                                           number, this switch will prevent the
                                           prompt.  NOTE: If a CVD is found in the
                                           --datadir its version+1 is used and
                                           this value is ignored.
    --no-cdiff                             Don't generate .cdiff file
    --unsigned                             Create unsigned database file (.cud)
    --print-certs=FILE                     Print Authenticode details from a PE
    --server=ADDR                          ClamAV Signing Service address
    --datadir=DIR                          Use DIR as default database directory
    --unpack=FILE          -u FILE         Unpack a CVD/CLD file
    --unpack-current=SHORTNAME             Unpack local CVD/CLD into cwd
    --list-sigs[=FILE]     -l[FILE]        List signature names
    --find-sigs=REGEX      -fREGEX         Find signatures matching REGEX
    --decode-sigs                          Decode signatures from stdin
    --test-sigs=DATABASE TARGET_FILE       Test signatures from DATABASE against 
                                           TARGET_FILE
    --vba=FILE                             Extract VBA/Word6 macro code
    --vba-hex=FILE                         Extract Word6 macro code with hex values
    --diff=OLD NEW         -d OLD NEW      Create diff for OLD and NEW CVDs
    --compare=OLD NEW      -c OLD NEW      Show diff between OLD and NEW files in
                                           cdiff format
    --run-cdiff=FILE       -r FILE         Execute update script FILE in cwd
    --verify-cdiff=DIFF CVD/CLD            Verify DIFF against CVD/CLD


~~~
