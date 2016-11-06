# simpdftex command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

This is simpdftex, 20070809

Usage: simpdftex formatname [--mode modestring]
	[--dvipsopts dvipsoptstring] [--extradvipsopts dvipsoptstring] [--pdf]
	[--default] [--maxpk] [--maxpfb] [--extendedname] [--no-echo-version]
	[--tex-path dir] [--keep-psfile] [--distiller-path dir] [--debug]
	[--distiller prog] [--distiller-filter prog] [--help]
	[--outdir dir] [--extratexopts texoptsstring]
	[--dvipdfmopts dvipdfmoptstring] tex-or-dvi-file

simpdftex is a way to do pdf{e}{la}tex without having pdf{e}{la}tex. It needs a
working TeX environment and one of three ways to turn  DVI file into PDF:
	- dvips + a distiller like ghostscript
	- dvipdfm
	- dvipdfmx
Since pdf{e}{la}tex cannot handle insertion of .eps graphics, simpdftex gives an
alternative when using dvips mode. The output for both systems is comparable.

simpdftex compiles the file with {LA}TeX, processes the DVI file with dvips into
PostScript and uses gs to produce pdf (with ps2pdf). Or it uses dvipdfm or
dvipdfmx to turn the DVI file into PDF. There is finegrained control over the
resulting filename and the options with which dvips produces the PostScript
intermediary file.

Dvips will call Metafont to produce bitmaps or include PostScript .pfb files
depending on the flags. See below.

The default setting is normal name, maximal use of pfb's, just like pdf{la}tex,
in other words, "pdftex file.tex" and "altpdftex file.tex" both produce an
output file file.pdf. For pdftex, output options are controlled by pdftex.cfg,
for altpdftext by config.ps (unless --pdf is given).

Arguments:
	tex-or-dvi-file
		If a .dvi file is given, skip the TeX process. Otherwise, TeX
		the input file, dvips the resulting dvi file and ps2pdf the
		resulting ps file
	--mode
		Tell simpdftex how to go from DVI to PDF. There are three modes:
		- dvips
		- dvipdfm
		- dvipdfmx
	--dpx
		Compatibility flag with simpdftex_dpmx. Equal to --mode dvipdfmx
	--dpm
		Compatibility flag with simpdftex_dpmx. Equal to --mode dvipdfm
	--help
		Display this message and exit
	--no-echo-version
		Do not echo location and version of this script. Does not exit
		so can be used tochange info to the output of a real run
	--debug
		Add some debug output
	--extendedname
		Depending on the mode, adds intermediary extensions to the
		output filename. If the mode is --pdf, .pdfmode is added. If
		the mode is --maxpk, ,maxpk is added and if the mode is
		--maxpfb, .maxpfb is added. Example:
			tex-or-dvi-file-basename.maxpfb.pdf
	--maxpk
		Use Metafont bitmaps (pk files) when possible. Only real
		PostScript fonts (like Times Roman) are included as
		PostScript fonts. All other fonts are included as bitmaps
		for the default printer resolution. This options produces
		optimal results for the chosen printer.
		For file contents (not name) equivalent to:
		--dvipsopts "-Ppk"
		Not yet functional for the other modes.
	--maxpfb
		Use PostScript pfb files whenever possible. This produces
		optimal results for the screen.
		For file contents (not name) equivalent to:
		--dvipsopts "-Poutline"
		If any font is included as TeX pk bitmap, it is rendered
		at the default resolution.
		Not yet functional for the other modes.
	--pdf
		Select .pdfmode extension for the output file name if
		--extendedname has been set. Use printer definition
		config.pdf. For file contents (not name) equivalent to
		--dvipsopts "-Ppdf"
		Note that the default config.pdf assumes resolution 8000
		for bitmaps and bitmap generation fails at this resolution
		because there exists no known mode for that resolution.
	--default
		Select no extension for the output file name, even if
		--extendedfilename has been set. Use standard printer
		definition config.ps. For file contents (not name) equivalent
		to:
		--dvipsopts "" --noextendedname
	--dvipsopts
		Give arbitrary arguments to dvips, e.g.
		--dvipsopts "-M"
		Sets extension for --extendedfilename to .custom. --dvipsopts
		overrides other flags that set dvipsopts.
	--extratexopts
		Give extra arbitrary arguments to tex, e.g.
		--extratexopts "--interaction=nonstopmode"
		Sets extra options for the tex command that is used.
	--extradvipsopts
		Give extra arbitrary arguments to dvips, e.g.
		--extradvipsopts "-M"
		Sets extra options for dvips and does not set extension
		or override other options. Options will be added to the end
		of the options for dvips
	--keep-psfile
		After running dvips, copy the ps file over to the directory
		where the tex file is, possibly overwriting a ps file
		that is there. Use with caution, a ps file could be input
		as well.
	--tex-path
		Give path of TeX binaries, use directory of this script
		otherwise
	--distiller prog
		Use a distiller different from ps2pdf which is the default.
		Argument must be an executable or executable script that
		gets called iwth two arguments: input file (PS) and output
		file (PDF). E.g.:
		--distiller=/usr/local/alternate/bin/ps2pdf
		--distiller=pstill
		Using this flag sets the distiller filter mode to off
		This flag only makes sense in dvips mode
	--distiller-filter prog
		Use a distiller executable or executable script which is
		called with the PS input as standard input and which writes
		the PDF output to standard output. E.g.:
		--distiller-filter=u-psbuild
		This flag only makes sense in dvips mode
	--distiller-path
		Give path needed by the distiller binary. This path is added
		to the begin of you PATH environment before the distiller is
		run. The reason is that for instance ps2pdf uses the path to
		find gs and sets the path to something with /sw/bin at the
		beginning.  Thus, installing gs from fink would make
		/usr/local/bin/ps2pdf find another gs than intended. By giving
		an empty path, the path is not changed before the distiller
		program is run. The default is empty.
		This flag only makes sense in dvips mode
	--dvipdfmopts
		Give arbitrary arguments to dvipdfm or dvipdfmx, e.g.
		--dvipdfmopts "-c"
		Sets extension for --extendedfilename to .custom. --dvipdfmopts
		overrides other flags that set dvipdfmopts.
	--outdir dir
		Write files here *if* our current directory is unwritable. This
		mimicks the TEXMFOUTPUT environment variable of TeX, but
		differently. The current dir becomes the value of --outdir and
		the directory where the old current dir is added to TEXINPUTS.
		This is more robust for reading and locating files.
		You can also set TEXMFOUTPUT instead, but with a disadvantage:
		you will be running TeXin the current dir. And you will not be
		able to read files in the outdir unless you also adapt
		TEXINPUTS.

	The defaults for the distiller are
		Path addition: "/usr/local/bin"
		Filter mode: "no"
		Program: "ps2pdf13"

	Later flags override settings of earlier flags.

~~~
