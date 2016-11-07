# affcopy command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

affcopy version 3.7.10
usage: affcopy [options] file1 file
                    Copies file1 to file2
       affcopy [options] file1 file2 file3 ... dir
                    Copies file1.. into dir
       affcopy [options] file1 file2 file3 ... dir1 dir2...
                    Copies file1.. into dirs1, dir2, ...

By default, all page MACs are verified on read and all segments
are verified after write.
Options:
   -v = verbose: print each file as it is copied
   -vv = very verbose: print each segment as it is copied
   -d = print debugging information as well
   -x = don't verify hashes on reads
   -y = don't verify writes
   -Xn = recompress pages (preen) with zlib level n
   -L  = recompress pages (preen) with LZMA (smaller but slower)

   -h = help; print this message.
   -V = print the program version and exit.
   -z = zap; copy even if the destination exists.
   -m = just copy the missing segments

Signature Options:
   -k filename.key   = specify private key for signing
   -c filename.cer   = specify a X.509 certificate that matches the private key
                       (by default, the file is assumed to be the same one
                       provided with the -k option.)
   -n  = read notes to accompany the copy from standard in.


Encryption Options:   Specify passphrase encryption for filename.aff with:
      file://:passphrase@/filename.aff

Examples:
       affcopy  file.aff   file://:mypassword@/file-encrypted.aff   - encrypt file.aff
       affcopy -vy -X9 *.aff s3:///     Copy all files in current
                               directory to S3 default bucket with X9 compression

~~~
