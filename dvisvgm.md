# dvisvgm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

dvisvgm (TeX Live) 1.15.1

This program converts DVI files, as created by TeX/LaTeX, to
the XML-based scalable vector graphics format SVG.

Usage: dvisvgm [options] dvifile
       dvisvgm -E [options] epsfile

Input options:
  -p, --page=ranges             choose pages to convert [1]
  -m, --fontmap=filenames       evaluate (additional) font map files
  -E, --eps                     convert an EPS file to SVG

SVG output options:
  -b, --bbox=size               set size of bounding box [min]
  -j, --clipjoin                compute intersection of clipping paths
      --colornames              prefer color names to RGB values if possible
      --comments                add comments with additional information
      --grad-overlap            create operlapping color gradient segments
      --grad-segments=number    number of color gradient segments per row [20]
      --grad-simplify=delta     reduce level of detail for small segments [0.05]
  -L, --linkmark=style          select how to mark hyperlinked areas [box]
  -o, --output=pattern          set name pattern of output files
  -d, --precision=number        set number of decimal points (0-6) [0]
  -R, --relative                create relative path commands
  -s, --stdout                  write SVG output to stdout
  -n, --no-fonts[=variant]      draw glyphs by using path elements [0]
      --no-merge                don't merge adjacent text elements
      --no-styles               don't use styles to reference fonts
  -z, --zip[=level]             create compressed .svgz file [9]

SVG transformations:
  -r, --rotate=angle            rotate page content clockwise
  -c, --scale=sx[,sy]           scale page content
  -t, --translate=tx[,ty]       shift page content
  -T, --transform=commands      transform page content
  -Z, --zoom=factor             zoom page content [1.0]

Processing options:
  -C, --cache[=dir]             set/print path of cache directory
  -e, --exact                   compute exact glyph boxes
      --keep                    keep temporary files
  -M, --mag=factor              magnification of Metafont output [4]
      --no-mktexmf              don't try to create missing fonts
  -S, --no-specials[=prefixes]  don't process [selected] specials
  -a, --trace-all[=retrace]     trace all glyphs of bitmap fonts [no]

Message options:
      --color                   colorize messages
  -h, --help[=mode]             print this summary of options and exit [0]
  -l, --list-specials           print supported special sets and exit
  -P, --progress[=delay]        enable progess indicator [0.5]
  -v, --verbosity=level         set verbosity level (0-7) [7]
  -V, --version[=extended]      print version and exit [no]

Copyright (C) 2005-2016 Martin Gieseking <martin.gieseking@uos.de> 


~~~
