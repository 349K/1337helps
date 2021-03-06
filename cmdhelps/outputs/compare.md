# compare command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Version: ImageMagick 6.8.9-9 Q16 x86_64 2016-09-25 http://www.imagemagick.org
Copyright: Copyright (C) 1999-2014 ImageMagick Studio LLC
Features: DPC Modules OpenMP
Delegates: bzlib djvu fftw fontconfig freetype jbig jng jpeg lcms lqr ltdl lzma openexr pangocairo png tiff wmf x xml zlib

Usage: compare [options ...] image reconstruct difference

Image Settings:
  -alpha option        on, activate, off, deactivate, set, opaque, copy
                       transparent, extract, background, or shape
  -authenticate password
                       decipher image with this password
  -channel type        apply option to select image channels
  -colorspace type     alternate image colorspace
  -compose operator    set image composite operator
  -compress type       type of pixel compression when writing the image
  -decipher filename   convert cipher pixels to plain pixels
  -define format:option
                       define one or more image format options
  -density geometry    horizontal and vertical density of the image
  -depth value         image depth
  -dissimilarity-threshold value
                       maximum distortion for (sub)image match
  -encipher filename   convert plain pixels to cipher pixels
  -extract geometry    extract area from image
  -format "string"     output formatted image characteristics
  -fuzz distance       colors within this distance are considered equal
  -highlight-color color
                       empasize pixel differences with this color
  -identify            identify the format and characteristics of the image
  -interlace type      type of image interlacing scheme
  -limit type value    pixel cache resource limit
  -lowlight-color color
                       de-emphasize pixel differences with this color
  -metric type         measure differences between images with this metric
  -monitor             monitor progress
  -passphrase filename get the passphrase from this file
  -profile filename    add, delete, or apply an image profile
  -quality value       JPEG/MIFF/PNG compression level
  -quiet               suppress all warning messages
  -quantize colorspace reduce colors in this colorspace
  -regard-warnings     pay attention to warning messages
  -respect-parentheses settings remain in effect until parenthesis boundary
  -sampling-factor geometry
                       horizontal and vertical sampling factor
  -seed value          seed a new sequence of pseudo-random numbers
  -set attribute value set an image attribute
  -quality value       JPEG/MIFF/PNG compression level
  -similarity-threshold value
                       minimum distortion for (sub)image match
  -size geometry       width and height of image
  -subimage-search     search for subimage
  -synchronize         synchronize image to storage device
  -taint               declare the image as modified
  -transparent-color color
                       transparent color
  -type type           image type
  -verbose             print detailed information about the image
  -version             print version information
  -virtual-pixel method
                       virtual pixel access method

Miscellaneous Options:
  -debug events        display copious debugging information
  -help                print program options
  -list type           print a list of supported option arguments
  -log format          format of debugging information

By default, the image format of `file' is determined by its magic
number.  To specify a particular image format, precede the filename
with an image format name and a colon (i.e. ps:image) or specify the
image type as the filename suffix (i.e. image.ps).  Specify 'file' as
'-' for standard input or output.

~~~
