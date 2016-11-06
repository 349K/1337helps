# updmap command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

updmap version r41566 (2016-06-29 18:04:35 +0200)
Usage: updmap     [OPTION] ... [COMMAND]
   or: updmap-sys [OPTION] ... [COMMAND]

Update the default font map files used by pdftex (pdftex.map), dvips
(psfonts.map), and dvipdfm(x), and optionally pxdvi, as determined by
all configuration files updmap.cfg (the ones returned by running
"kpsewhich --all updmap.cfg", but see below).

Among other things, these map files are used to determine which fonts
should be used as bitmaps and which as outlines, and to determine which
font files are included, typically subsetted, in the PDF or PostScript output.

updmap-sys is intended to affect the system-wide configuration, while
updmap affects personal configuration files only, overriding the system
files.  As a consequence, once updmap has been run, even a single time,
running updmap-sys no longer has any effect.  (updmap-sys issues a
warning in this situation.)

By default, the TeX filename database (ls-R) is also updated.

The updmap system is regrettably complicated, for both inherent and
historical reasons.  A general overview:
- updmap.cfg files are mainly about listing other files, namely the
  font-specific .maps, in which each line gives information about a
  different TeX (.tfm) font.
- updmap reads the updmap.cfg files and then concatenates the
  contents of those .map files into the main output files: psfonts.map
  for dvips and pdftex.map for pdftex and dvipdfmx.
- The updmap.cfg files themselves are created and updated at package
  installation time, by the system installer or the package manager or
  by hand, and not (by default) by updmap.

Good luck.

Options:
  --cnffile FILE            read FILE for the updmap configuration 
                             (can be given multiple times, in which case
                             all the files are used)
  --dvipdfmxoutputdir DIR   specify output directory (dvipdfm(x) syntax)
  --dvipsoutputdir DIR      specify output directory (dvips syntax)
  --pdftexoutputdir DIR     specify output directory (pdftex syntax)
  --pxdvioutputdir DIR      specify output directory (pxdvi syntax)
  --outputdir DIR           specify output directory (for all files)
  --copy                    cp generic files rather than using symlinks
  --force                   recreate files even if config hasn't changed
  --nomkmap                 do not recreate map files
  --nohash                  do not run texhash
  --sys                     affect system-wide files (equivalent to updmap-sys)
  -n, --dry-run             only show the configuration, no output
  --quiet, --silent         reduce verbosity

Commands:
  --help                    show this message and exit
  --version                 show version information and exit
  --showoption OPTION       show the current setting of OPTION
  --showoptions OPTION      show possible settings for OPTION
  --setoption OPTION VALUE  set OPTION to value; option names below
  --setoption OPTION=VALUE  as above, just different syntax
  --enable MAPTYPE MAPFILE  add "MAPTYPE MAPFILE" to updmap.cfg,
                             where MAPTYPE is Map, MixedMap, or KanjiMap
  --enable Map=MAPFILE      add "Map MAPFILE" to updmap.cfg
  --enable MixedMap=MAPFILE add "MixedMap MAPFILE" to updmap.cfg
  --enable KanjiMap=MAPFILE add "KanjiMap MAPFILE" to updmap.cfg
  --disable MAPFILE         disable MAPFILE, of whatever type
  --listmaps                list all maps (details below)
  --listavailablemaps       list available maps (details below)
  --syncwithtrees           disable unavailable map files in updmap.cfg

The main output:

  The main output of updmap is the files containing the individual font
  map lines which the drivers (dvips, pdftex, etc.) read to handle fonts.
  
  The map files for dvips (psfonts.map) and pdftex and dvipdfmx
  (pdftex.map) are written to TEXMFVAR/fonts/map/updmap/{dvips,pdftex}/.
  
  In addition, information about Kanji fonts is written to
  TEXMFVAR/fonts/map/updmap/dvipdfmx/kanjix.map, and optionally to 
  TEXMFVAR/fonts/map/updmap/pxdvi/xdvi-ptex.map.  These are for Kanji
  only and are not like other map files.  dvipdfmx reads pdftex.map for
  the map entries for non-Kanji fonts.
  
  If no option is given, so the invocation is just "updmap" or
  "updmap-sys", these output files are always recreated.

  Otherwise, if an option such as --enable or --disable is given, the
  output files are recreated if the list of enabled map files (from
  updmap.cfg) has changed.  The --force option overrides this,
  always recreating the output files.
  
Explanation of the map types:

  The normal type is Map.
  
  The only difference between Map and MixedMap is that MixedMap entries
  are not added to psfonts_pk.map.  The purpose is to help users with
  devices that render Type 1 outline fonts worse than mode-tuned Type 1
  bitmap fonts.  So, MixedMap is used for fonts that are available as
  both Type 1 and Metafont.

  KanjiMap entries are added to psfonts_t1.map and kanjix.map.

Explanation of the OPTION names for --showoptions, --showoption, --setoption:

  dvipsPreferOutline    true,false  (default true)
    Whether dvips uses bitmaps or outlines, when both are available.
  dvipsDownloadBase35   true,false  (default true)
    Whether dvips includes the standard 35 PostScript fonts in its output.
  pdftexDownloadBase14  true,false   (default true)
    Whether pdftex includes the standard 14 PDF fonts in its output.
  pxdviUse              true,false  (default false)
    Whether maps for pxdvi (Japanese-patched xdvi) are under updmap's control.
  kanjiEmbed            (any string)
  kanjiVariant          (any string)
    See below.
  LW35                  URWkb,URW,ADOBEkb,ADOBE  (default URWkb)
    Adapt the font and file names of the standard 35 PostScript fonts.

    URWkb    URW fonts with "berry" filenames    (e.g. uhvbo8ac.pfb)
    URW      URW fonts with "vendor" filenames   (e.g. n019064l.pfb)
    ADOBEkb  Adobe fonts with "berry" filenames  (e.g. phvbo8an.pfb)
    ADOBE    Adobe fonts with "vendor" filenames (e.g. hvnbo___.pfb)

  These options are only read and acted on by updmap; dvips, pdftex, etc.,
  do not know anything about them.  They work by changing the default map
  file which the programs read, so they can be overridden by specifying
  command-line options or configuration files to the programs, as
  explained at the beginning of updmap.cfg.

  The options kanjiEmbed and kanjiVariant specify special replacements
  in the map lines.  If a map contains the string @kanjiEmbed@, then
  this will be replaced by the value of that option; similarly for
  kanjiVariant.  In this way, users of Japanese TeX can select different
  fonts to be included in the final output.

Explanation of trees and files normally used:

  If --cnffile is specified on the command line (can be given multiple
  times), its value(s) is(are) used.  Otherwise, updmap reads all the
  updmap.cfg files found by running `kpsewhich -all updmap.cfg',
  in the order returned by kpsewhich (which is the order of trees
  defined in texmf.cnf).

  In either case, if multiple updmap.cfg files are found, all the maps
  mentioned in all the updmap.cfg files are merged.

  Thus, if updmap.cfg files are present in all trees, and the default
  layout is used as shipped with TeX Live, the following files are
  read, in the given order.
  
  For updmap-sys:
  TEXMFSYSCONFIG $TEXLIVE/YYYY/texmf-config/web2c/updmap.cfg
  TEXMFSYSVAR    $TEXLIVE/YYYY/texmf-var/web2c/updmap.cfg
  TEXMFLOCAL     $TEXLIVE/texmf-local/web2c/updmap.cfg
  TEXMFDIST      $TEXLIVE/YYYY/texmf-dist/web2c/updmap.cfg

  For updmap:
  TEXMFCONFIG    $HOME/.texliveYYYY/texmf-config/web2c/updmap.cfg
  TEXMFVAR       $HOME/.texliveYYYY/texmf-var/web2c/updmap.cfg
  TEXMFHOME      $HOME/texmf/web2c/updmap.cfg
  TEXMFSYSCONFIG $TEXLIVE/YYYY/texmf-config/web2c/updmap.cfg
  TEXMFSYSVAR    $TEXLIVE/YYYY/texmf-var/web2c/updmap.cfg
  TEXMFLOCAL     $TEXLIVE/texmf-local/web2c/updmap.cfg
  TEXMFDIST      $TEXLIVE/YYYY/texmf-dist/web2c/updmap.cfg
  
  (where YYYY is the TeX Live release version).
  
  According to the actions, updmap might write to one of the given files
  or create a new updmap.cfg, described further below.

Where and which updmap.cfg changes are saved: 

  When no options are given, the updmap.cfg file(s) are only read, not
  written.  It's when an option --setoption, --enable or --disable is
  specified that an updmap.cfg needs to be updated.  In this case:

  1) If config files are given on the command line, then the first one
  given is used to save any such changes.
  
  2) If the config files are taken from kpsewhich output, then the
  algorithm is more complex:

    2a) If $TEXMFCONFIG/web2c/updmap.cfg or $TEXMFHOME/web2c/updmap.cfg
    appears in the list of used files, then the one listed first by
    kpsewhich --all (equivalently, the one returned by kpsewhich
    updmap.cfg), is used.
      
    2b) If neither of the above two are present and changes are made, a
    new config file is created in $TEXMFCONFIG/web2c/updmap.cfg.
  
  In general, the idea is that if the user cannot write to a given
  config file, a higher-level one can be used.  That way, the
  distribution's settings can be overridden system-wide using
  TEXMFLOCAL, and system settings can be overridden again in a
  particular user's TEXMFHOME.

Resolving multiple definitions of a font:

  If a font is defined in more than one map file, then the definition
  coming from the first-listed updmap.cfg is used.  If a font is
  defined multiple times within the same map file, one is chosen
  arbitrarily.  In both cases a warning is issued.

Disabling maps:

  updmap.cfg files with higher priority (listed earlier) can disable
  maps mentioned in lower priority (listed later) updmap.cfg files by
  writing, e.g.,
    #! Map mapname.map
  or
    #! MixedMap mapname.map
  in the higher-priority updmap.cfg file.  (The #! must be at the
  beginning of the line, with at least one space or tab afterward, and
  whitespace between each word on the list.)

  As an example, suppose you have a copy of MathTime Pro fonts
  and want to disable the Belleek version of the fonts; that is,
  disable the map belleek.map.  You can create the file
  $TEXMFCONFIG/web2c/updmap.cfg with the content
    #! Map belleek.map
    Map mt-plus.map
    Map mt-yy.map
  and call updmap.

Listing of maps:

  The two options --listmaps and --listavailablemaps list all maps
  defined in any of the updmap.cfg files (for --listmaps), and 
  only those actually found on the system (for --listavailablemaps).
  The output format is one line per font map, with the following
  fields separated by tabs: map, type (Map, MixedMap, KanjiMap),
  status (enabled, disabled), origin (the updmap.cfg file where
  it is mentioned, or 'builtin' for the three basic maps).

  In the case of --listmaps there can be one additional fields
  (again separated by tab) containing '(not available)' for those
  map files that cannot be found.
 
updmap vs. updmap-sys:

  When updmap-sys is run, TEXMFSYSCONFIG and TEXMFSYSVAR are used
  instead of TEXMFCONFIG and TEXMFVAR, respectively.  This is the
  primary difference between updmap-sys and updmap.

  Other locations may be used if you give them on the command line, or
  these trees don't exist, or you are not using the original TeX Live.

To see the precise locations of the various files that
will be read and written, give the -n option (or read the source).

The log file is written to TEXMFVAR/web2c/updmap.log.

For step-by-step instructions on making new fonts known to TeX, read
http://tug.org/fonts/fontinstall.html.  For even more terse
instructions, read the beginning of the main updmap.cfg file.

Report bugs to: tex-live@tug.org
TeX Live home page: <http://tug.org/texlive/>

~~~
