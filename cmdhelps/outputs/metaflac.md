# metaflac command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

==============================================================================
metaflac - Command-line FLAC metadata editor version 1.3.1
Copyright (C) 2001-2009  Josh Coalson
Copyright (C) 2011-2014  Xiph.Org Foundation

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
==============================================================================

Usage:
  metaflac [options] [operations] FLACfile [FLACfile ...]

Use metaflac to list, add, remove, or edit metadata in one or more FLAC files.
You may perform one major operation, or many shorthand operations at a time.

Options:
--preserve-modtime    Preserve the original modification time in spite of edits
--with-filename       Prefix each output line with the FLAC file name
                      (the default if more than one FLAC file is specified)
--no-filename         Do not prefix each output line with the FLAC file name
                      (the default if only one FLAC file is specified)
--no-utf8-convert     Do not convert tags from UTF-8 to local charset,
                      or vice versa.  This is useful for scripts, and setting
                      tags in situations where the locale is wrong.
--dont-use-padding    By default metaflac tries to use padding where possible
                      to avoid rewriting the entire file if the metadata size
                      changes.  Use this option to tell metaflac to not take
                      advantage of padding this way.

Shorthand operations:
--show-md5sum         Show the MD5 signature from the STREAMINFO block.
--show-min-blocksize  Show the minimum block size from the STREAMINFO block.
--show-max-blocksize  Show the maximum block size from the STREAMINFO block.
--show-min-framesize  Show the minimum frame size from the STREAMINFO block.
--show-max-framesize  Show the maximum frame size from the STREAMINFO block.
--show-sample-rate    Show the sample rate from the STREAMINFO block.
--show-channels       Show the number of channels from the STREAMINFO block.
--show-bps            Show the # of bits per sample from the STREAMINFO block.
--show-total-samples  Show the total # of samples from the STREAMINFO block.

--show-vendor-tag     Show the vendor string from the VORBIS_COMMENT block.
--show-tag=NAME       Show all tags where the the field name matches 'NAME'.
--remove-tag=NAME     Remove all tags whose field name is 'NAME'.
--remove-first-tag=NAME  Remove first tag whose field name is 'NAME'.
--remove-all-tags     Remove all tags, leaving only the vendor string.
--set-tag=FIELD       Add a tag.  The FIELD must comply with the Vorbis comment
                      spec, of the form "NAME=VALUE".  If there is currently
                      no tag block, one will be created.
--set-tag-from-file=FIELD   Like --set-tag, except the VALUE is a filename
                      whose contents will be read verbatim to set the tag value.
                      Unless --no-utf8-convert is specified, the contents will
                      be converted to UTF-8 from the local charset.  This can
                      be used to store a cuesheet in a tag (e.g.
                      --set-tag-from-file="CUESHEET=image.cue").  Do not try
                      to store binary data in tag fields!  Use APPLICATION
                      blocks for that.
--import-tags-from=FILE Import tags from a file.  Use '-' for stdin.  Each line
                      should be of the form NAME=VALUE.  Multi-line comments
                      are currently not supported.  Specify --remove-all-tags
                      and/or --no-utf8-convert before --import-tags-from if
                      necessary.  If FILE is '-' (stdin), only one FLAC file
                      may be specified.
--export-tags-to=FILE Export tags to a file.  Use '-' for stdout.  Each line
                      will be of the form NAME=VALUE.  Specify
                      --no-utf8-convert if necessary.
--import-cuesheet-from=FILE  Import a cuesheet from a file.  Use '-' for stdin.
                      Only one FLAC file may be specified.  A seekpoint will be
                      added for each index point in the cuesheet to the
                      SEEKTABLE unless --no-cued-seekpoints is specified.
--export-cuesheet-to=FILE  Export CUESHEET block to a cuesheet file, suitable
                      for use by CD authoring software.  Use '-' for stdout.
                      Only one FLAC file may be specified on the command line.
--import-picture-from=FILENAME|SPECIFICATION  Import a picture and store it in a
                      PICTURE block.  Either a filename for the picture file or
                      a more complete specification form can be used.  The
                      SPECIFICATION is a string whose parts are separated by |
                      characters.  Some parts may be left empty to invoke
                      default values.  FILENAME is just shorthand for
                      "||||FILENAME".  The format of SPECIFICATION is:
         [TYPE]|[MIME-TYPE]|[DESCRIPTION]|[WIDTHxHEIGHTxDEPTH[/COLORS]]|FILE
           TYPE is optional; it is a number from one of:
              0: Other
              1: 32x32 pixels 'file icon' (PNG only)
              2: Other file icon
              3: Cover (front)
              4: Cover (back)
              5: Leaflet page
              6: Media (e.g. label side of CD)
              7: Lead artist/lead performer/soloist
              8: Artist/performer
              9: Conductor
             10: Band/Orchestra
             11: Composer
             12: Lyricist/text writer
             13: Recording Location
             14: During recording
             15: During performance
             16: Movie/video screen capture
             17: A bright coloured fish
             18: Illustration
             19: Band/artist logotype
             20: Publisher/Studio logotype
             The default is 3 (front cover).  There may only be one picture each
             of type 1 and 2 in a file.
           MIME-TYPE is optional; if left blank, it will be detected from the
             file.  For best compatibility with players, use pictures with MIME
             type image/jpeg or image/png.  The MIME type can also be --> to
             mean that FILE is actually a URL to an image, though this use is
             discouraged.
           DESCRIPTION is optional; the default is an empty string
           The next part specfies the resolution and color information.  If
             the MIME-TYPE is image/jpeg, image/png, or image/gif, you can
             usually leave this empty and they can be detected from the file.
             Otherwise, you must specify the width in pixels, height in pixels,
             and color depth in bits-per-pixel.  If the image has indexed colors
             you should also specify the number of colors used.
           FILE is the path to the picture file to be imported, or the URL if
             MIME type is -->
--export-picture-to=FILE  Export PICTURE block to a file.  Use '-' for stdout.
                      Only one FLAC file may be specified.  The first PICTURE
                      block will be exported unless --export-picture-to is
                      preceded by a --block-number=# option to specify the exact
                      metadata block to extract.  Note that the block number is
                      the one shown by --list.
--add-replay-gain     Calculates the title and album gains/peaks of the given
                      FLAC files as if all the files were part of one album,
                      then stores them in the VORBIS_COMMENT block.  The tags
                      are the same as those used by vorbisgain.  Existing
                      ReplayGain tags will be replaced.  If only one FLAC file
                      is given, the album and title gains will be the same.
                      Since this operation requires two passes, it is always
                      executed last, after all other operations have been
                      completed and written to disk.  All FLAC files specified
                      must have the same resolution, sample rate, and number
                      of channels.  The sample rate must be one of 8, 11.025,
                      12, 16, 22.05, 24, 32, 44.1, or 48 kHz.
--remove-replay-gain  Removes the ReplayGain tags.
--add-seekpoint={#|X|#x|#s}  Add seek points to a SEEKTABLE block
       #  : a specific sample number for a seek point
       X  : a placeholder point (always goes at the end of the SEEKTABLE)
       #x : # evenly spaced seekpoints, the first being at sample 0
       #s : a seekpoint every # seconds; # does not have to be a whole number
                      If no SEEKTABLE block exists, one will be created.  If
                      one already exists, points will be added to the existing
                      table, and any duplicates will be turned into placeholder
                      points.  You may use many --add-seekpoint options; the
                      resulting SEEKTABLE will be the unique-ified union of
                      all such values.  Example: --add-seekpoint=100x
                      --add-seekpoint=3.5s will add 100 evenly spaced
                      seekpoints and a seekpoint every 3.5 seconds.
--add-padding=length  Add a padding block of the given length (in bytes).
                      The overall length of the new block will be 4 + length;
                      the extra 4 bytes is for the metadata block header.

Major operations:
--version
    Show the metaflac version number.
--list
    List the contents of one or more metadata blocks to stdout.  By default,
    all metadata blocks are listed in text format.  Use the following options
    to change this behavior:

    --block-number=#[,#[...]]
    An optional comma-separated list of block numbers to display.  The first
    block, the STREAMINFO block, is block 0.

    --block-type=type[,type[...]]
    --except-block-type=type[,type[...]]
    An optional comma-separated list of block types to be included or ignored
    with this option.  Use only one of --block-type or --except-block-type.
    The valid block types are: STREAMINFO, PADDING, APPLICATION, SEEKTABLE,
    VORBIS_COMMENT.  You may narrow down the types of APPLICATION blocks
    displayed as follows:
        APPLICATION:abcd        The APPLICATION block(s) whose textual repre-
                                sentation of the 4-byte ID is "abcd"
        APPLICATION:0xXXXXXXXX  The APPLICATION block(s) whose hexadecimal big-
                                endian representation of the 4-byte ID is
                                "0xXXXXXXXX".  For the example "abcd" above the
                                hexadecimal equivalalent is 0x61626364

    NOTE: if both --block-number and --[except-]block-type are specified,
          the result is the logical AND of both arguments.

    --application-data-format=hexdump|text
    If the application block you are displaying contains binary data but your
    --data-format=text, you can display a hex dump of the application data
    contents instead using --application-data-format=hexdump

--remove
    Remove one or more metadata blocks from the metadata.  Unless
    --dont-use-padding is specified, the blocks will be replaced with padding.
    You may not remove the STREAMINFO block.

    --block-number=#[,#[...]]
    --block-type=type[,type[...]]
    --except-block-type=type[,type[...]]
    See --list above for usage.

    NOTE: if both --block-number and --[except-]block-type are specified,
          the result is the logical AND of both arguments.

--remove-all
    Remove all metadata blocks (except the STREAMINFO block) from the
    metadata.  Unless --dont-use-padding is specified, the blocks will be
    replaced with padding.

--merge-padding
    Merge adjacent PADDING blocks into single blocks.

--sort-padding
    Move all PADDING blocks to the end of the metadata and merge them into a
    single block.

~~~
