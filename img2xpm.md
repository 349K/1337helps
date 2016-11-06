# img2xpm command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



img2xpm.py  -- convert several image formats to XPM.

Usage:

    img2xpm.py [options] image_files...

Options:

    -o <dir>       The directory to place the .xpm file(s), defaults to
                   the current directory.

    -m <#rrggbb>   If the original image has a mask or transparency defined
                   it will be used by default.  You can use this option to
                   override the default or provide a new mask by specifying
                   a colour in the image to mark as transparent.

    -n <name>      A filename to write the .xpm data to.  Defaults to the
                   basename of the image file + '.xpm'  This option overrides
                   the -o option.


~~~
