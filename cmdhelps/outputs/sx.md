# sx command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

sx version 0.12.21rc
Usage: sx [options] file ...
   or: sx [options] -{c|i} COMMAND
Send file(s) with ZMODEM/YMODEM/XMODEM protocol
    (X) = option applies to XMODEM only
    (Y) = option applies to YMODEM only
    (Z) = option applies to ZMODEM only
  -+, --append                append to existing destination file (Z)
  -2, --twostop               use 2 stop bits
  -4, --try-4k                go up to 4K blocksize
      --start-4k              start with 4K blocksize (doesn't try 8)
  -8, --try-8k                go up to 8K blocksize
      --start-8k              start with 8K blocksize
  -a, --ascii                 ASCII transfer (change CR/LF to LF)
  -b, --binary                binary transfer
  -B, --bufsize N             buffer N bytes (N==auto: buffer whole file)
  -c, --command COMMAND       execute remote command COMMAND (Z)
  -C, --command-tries N       try N times to execute a command (Z)
  -d, --dot-to-slash          change '.' to '/' in pathnames (Y/Z)
      --delay-startup N       sleep N seconds before doing anything
  -e, --escape                escape all control characters (Z)
  -E, --rename                force receiver to rename files it already has
  -f, --full-path             send full pathname (Y/Z)
  -i, --immediate-command CMD send remote CMD, return immediately (Z)
  -h, --help                  print this usage message
  -k, --1k                    send 1024 byte packets (X)
  -L, --packetlen N           limit subpacket length to N bytes (Z)
  -l, --framelen N            limit frame length to N bytes (l>=L) (Z)
  -m, --min-bps N             stop transmission if BPS below N
  -M, --min-bps-time N          for at least N seconds (default: 120)
  -n, --newer                 send file if source newer (Z)
  -N, --newer-or-longer       send file if source newer or longer (Z)
  -o, --16-bit-crc            use 16 bit CRC instead of 32 bit CRC (Z)
  -O, --disable-timeouts      disable timeout code, wait forever
  -p, --protect               protect existing destination file (Z)
  -r, --resume                resume interrupted file transfer (Z)
  -R, --restricted            restricted, more secure mode
  -q, --quiet                 quiet (no progress reports)
  -s, --stop-at {HH:MM|+N}    stop transmission at HH:MM or in N seconds
      --tcp-server            open socket, wait for connection (Z)
      --tcp-client ADDR:PORT  open socket, connect to ... (Z)
  -u, --unlink                unlink file after transmission
  -U, --unrestrict            turn off restricted mode (if allowed to)
  -v, --verbose               be verbose, provide debugging information
  -w, --windowsize N          Window is N bytes (Z)
  -X, --xmodem                use XMODEM protocol
  -y, --overwrite             overwrite existing files
  -Y, --overwrite-or-skip     overwrite existing files, else skip
      --ymodem                use YMODEM protocol
  -Z, --zmodem                use ZMODEM protocol

short options use the same arguments as the long ones

~~~
