# miniterm.py command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: miniterm.py [-h] [--parity {N,E,O,S,M}] [--rtscts] [--xonxoff]
                   [--rts RTS] [--dtr DTR] [--ask] [-e] [--encoding CODEC]
                   [-f NAME] [--eol {CR,LF,CRLF}] [--raw] [--exit-char NUM]
                   [--menu-char NUM] [-q] [--develop]
                   [port] [baudrate]

Miniterm - A simple terminal program for the serial port.

positional arguments:
  port                  serial port name ('-' to show port list)
  baudrate              set baud rate, default: 9600

optional arguments:
  -h, --help            show this help message and exit

port settings:
  --parity {N,E,O,S,M}  set parity, one of {N E O S M}, default: N
  --rtscts              enable RTS/CTS flow control (default off)
  --xonxoff             enable software flow control (default off)
  --rts RTS             set initial RTS line state (possible values: 0, 1)
  --dtr DTR             set initial DTR line state (possible values: 0, 1)
  --ask                 ask again for port when open fails

data handling:
  -e, --echo            enable local echo (default off)
  --encoding CODEC      set the encoding for the serial port (e.g. hexlify,
                        Latin1, UTF-8), default: UTF-8
  -f NAME, --filter NAME
                        add text transformation
  --eol {CR,LF,CRLF}    end of line mode
  --raw                 Do no apply any encodings/transformations

hotkeys:
  --exit-char NUM       Unicode of special character that is used to exit the
                        application, default: 29
  --menu-char NUM       Unicode code of special character that is used to
                        control miniterm (menu), default: 20

diagnostics:
  -q, --quiet           suppress non-error messages
  --develop             show Python traceback on error

~~~
