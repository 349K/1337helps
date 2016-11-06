# mktexpk command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: mktexpk [OPTIONS] NAME [REDIRECT],
  Create a PK font.

--dpi DPI           use resolution DPI.
--bdpi BDPI         use base resolution BDPI.
--mag MAG           use magnificiation MAG.
--mfmode MODE       use MODE as the METAFONT mode.
--destdir DESTDIR   write fonts in DESTDIR.

Try to create a bitmap PK file for NAME at resolution DPI, with an
assumed device base resolution of BDPI, and a Metafont `mag' of
MAG. Use MODE for the METAFONT mode.  Use DESTDIR for the root of where
to install into, either the absolute directory name to use (if it starts
with a /) or relative to the default DESTDIR (if not). REDIRECT, if
supplied, is a string of the form '>&n', where n is the number of the
file descriptor which is to receive, instead of stdout, the name of the
newly created pk file.

If you expected the font to be available as an outline, and thus this
script does not work and should not have been called, most likely the
font's .tfm name is missing from the relevant map file (e.g.,
psfonts.map for dvips, pdftex.map for pdftex).  These map files are
typically maintained using updmap; q.v.

For step-by-step instructions on making new fonts known to TeX, see
http://tug.org/fonts/fontinstall.html.

Report bugs to: tex-k@tug.org
TeX Live home page: <http://tug.org/texlive/>


~~~
