# totem-video-thumbnailer command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
  totem-video-thumbnailer [OPTION...] [INPUT FILE] [OUTPUT FILE] Thumbnail movies

Help Options:
  -h, --help                        Show help options
  --help-all                        Show all help options
  --help-gst                        Show GStreamer Options

Application Options:
  -j, --jpeg                        Output the thumbnail as a JPEG instead of PNG
  -s, --size                        Size of the thumbnail in pixels (with --gallery sets the size of individual screenshots)
  -r, --raw                         Output the raw picture of the video without scaling or adding borders
  -l, --no-limit                    Don't limit the thumbnailing time to 30 seconds
  -v, --verbose                     Output debug information
  -t, --time                        Choose this time (in seconds) as the thumbnail (can't be used with --gallery)
  --g-fatal-warnings                Make all warnings fatal
  -g, --gallery                     Output a gallery of the given number (0 is default) of screenshots (can't be used with --time)
  -p, --print-progress              Only print progress updates (can't be used with --verbose)


~~~
