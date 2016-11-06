# tjbench command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


USAGE: tjbench
       <Inputfile (BMP|PPM)> <Quality> [options]

       tjbench
       <Inputfile (JPG)> [options]

Options:

-alloc = Dynamically allocate JPEG image buffers
-bmp = Generate output images in Windows Bitmap format (default = PPM)
-bottomup = Test bottom-up compression/decompression
-tile = Test performance of the codec when the image is encoded as separate
     tiles of varying sizes.
-rgb, -bgr, -rgbx, -bgrx, -xbgr, -xrgb =
     Test the specified color conversion path in the codec (default = BGR)
-cmyk = Indirectly test YCCK JPEG compression/decompression (the source
     and destination bitmaps are still RGB.  The conversion is done
     internally prior to compression or after decompression.)
-fastupsample = Use the fastest chrominance upsampling algorithm available in
     the underlying codec
-fastdct = Use the fastest DCT/IDCT algorithms available in the underlying
     codec
-accuratedct = Use the most accurate DCT/IDCT algorithms available in the
     underlying codec
-subsamp <s> = When testing JPEG compression, this option specifies the level
     of chrominance subsampling to use (<s> = 444, 422, 440, 420, 411, or
     GRAY).  The default is to test Grayscale, 4:2:0, 4:2:2, and 4:4:4 in
     sequence.
-quiet = Output results in tabular rather than verbose format
-yuv = Test YUV encoding/decoding functions
-yuvpad <p> = If testing YUV encoding/decoding, this specifies the number of
     bytes to which each row of each plane in the intermediate YUV image is
     padded (default = 1)
-scale M/N = Scale down the width/height of the decompressed JPEG image by a
     factor of M/N (M/N = 2/1, 15/8, 7/4, 13/8, 3/2, 11/8, 5/4, 9/8, 1/1, 
     7/8, 3/4, 5/8, 1/2, 3/8, 1/4, or 1/8)
-hflip, -vflip, -transpose, -transverse, -rot90, -rot180, -rot270 =
     Perform the corresponding lossless transform prior to
     decompression (these options are mutually exclusive)
-grayscale = Perform lossless grayscale conversion prior to decompression
     test (can be combined with the other transforms above)
-benchtime <t> = Run each benchmark for at least <t> seconds (default = 5.0)
-warmup <w> = Execute each benchmark <w> times to prime the cache before
     taking performance measurements (default = 1)
-componly = Stop after running compression tests.  Do not test decompression.
-nowrite = Do not write reference or output images (improves consistency of
     performance measurements.)

NOTE:  If the quality is specified as a range (e.g. 90-100), a separate
test will be performed for all quality values in the range.


~~~
