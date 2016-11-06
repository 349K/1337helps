# xdvipdfmx command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage: xdvipdfmx [OPTION]... [DVIFILE[.dvi|.xdv]]
       xdvipdfmx --extractbb|--xbb|--ebb [OPTION]...	Be "extractbb"
       xdvipdfmx --help|--showpaper|--version
Convert DVI or XDV input to PDF; defaults given below.

Options:
  -c 		Ignore color specials (for B&W printing)
  --dvipdfm	Enable DVIPDFM emulation mode
  -d number	Set PDF decimal digits (0-5) [3]
  -f filename	Set font map file name [pdftex.map]
  -g dimension	Annotation "grow" amount [0.0in]
  -h | --help 	Show this help message and exit
  -l 		Landscape mode
  -m number	Set additional magnification [1.0]
  --mvorigin	Translate the origin for MP inclusion
  -o filename	Set output file name, "-" for stdout [DVIFILE.pdf]
  -p papersize	Set papersize [a4]
  -q 		Be quiet
  -r resolution	Set resolution (in DPI) for raster fonts [600]
  -s pages	Select page ranges [all pages]
  --showpaper	Show available paper formats and exit
  -t 		Embed thumbnail images of PNG format [DVIFILE.1] 
  --version	Output version information and exit
  -v 		Be verbose
  -vv		Be more verbose
  --kpathsea-debug number	Set kpathsea debugging flags [0]
  -x dimension	Set horizontal offset [1.0in]
  -y dimension	Set vertical offset [1.0in]
  -z number  	Set zlib compression level (0-9) [9]
  -C number	Specify miscellaneous option flags [0]:
		  0x0001 reserved
		  0x0002 Use semi-transparent filling for tpic shading command,
			 instead of opaque gray color; requires PDF 1.4.
		  0x0004 Treat all CIDFont as fixed-pitch font.
		  0x0008 Do not replace duplicate fontmap entries.
		  0x0010 Do not optimize PDF destinations.
		  0x0020 Do not use predictor filter for Flate compression.
		  0x0040 Do not use object stream.
		Positive values are always ORed with previously given flags.
		And negative values replace old values.
  -D template	PS->PDF conversion command line template [none]
  -E 		Always try to embed fonts, regardless of licensing flags.
  -I number	Image cache life in hours [-2]
           	 0: erase all old images and leave new images
           	-1: erase all old images and also erase new images
           	-2: ignore image cache
  -K number	Encryption key length [40]
  -M 		Process MetaPost PostScript output
  -O number	Set maximum depth of open bookmark items [0]
  -P number	Set permission flags for PDF encryption [0x003C]
  -S 		Enable PDF encryption
  -V number	Set PDF minor version [5]

All dimensions entered on the command line are "true" TeX dimensions.
Argument of "-s" lists physical page ranges separated by commas,
	e.g., "-s 1-3,5-6".
Papersize is specified by paper format (e.g., "a4")
	or by w<unit>,h<unit> (e.g., "20cm,30cm").

Email bug reports to tex-k@tug.org.

~~~
