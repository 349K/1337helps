# python2-qr command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: qr - Convert stdin (or the first argument) to a QR Code.

When stdout is a tty the QR Code is printed to the terminal and when stdout is
a pipe to a file an image is written. The default image format is PNG.

Options:
  -h, --help            show this help message and exit
  --factory=FACTORY     Full python path to the image factory class to create
                        the image with. You can use the following shortcuts to
                        the built-in image factory classes: pil, pymaging,
                        svg, svg-fragment, svg-path.
  --optimize=OPTIMIZE   Optimize the data by looking for chunks of at least
                        this many characters that could use a more efficient
                        encoding method. Use 0 to turn off chunk optimization.
  --error-correction=ERROR_CORRECTION
                        The error correction level to use. Choices are L (7%),
                        M (15%, default), Q (25%), and H (30%).

~~~
