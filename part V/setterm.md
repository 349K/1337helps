# setterm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 setterm [options]

Set the attributes of a terminal.

Options:
 --term          <terminal_name>   override TERM environment variable
 --reset                           reset terminal to power-on state
 --initialize                      display init string, and use default settings
 --default                         use default terminal settings
 --store                           save current terminal settings as default
 --cursor        [on|off]          display cursor
 --repeat        [on|off]          keyboard repeat
 --appcursorkeys [on|off]          cursor key application mode
 --linewrap      [on|off]          continue on a new line when a line is full
 --inversescreen [on|off]          swap colors for the whole screen
 --foreground    default|<color>   set foreground color
 --background    default|<color>   set background color
 --ulcolor       [bright] <color>  set underlined text color
 --hbcolor       [bright] <color>  set bold text color
                 <color>: black blue cyan green grey magenta red white yellow
 --bold          [on|off]          bold
 --half-bright   [on|off]          dim
 --blink         [on|off]          blink
 --underline     [on|off]          underline
 --reverse       [on|off]          swap foreground and background colors
 --clear         [all|rest]        clear screen and set cursor position
 --tabs          [<number>...]     set these tab stop positions, or show them
 --clrtabs       [<number>...]     clear these tab stop positions, or all
 --regtabs       [1-160]           set a regular tab stop interval
 --blank         [0-60|force|poke] set time of inactivity before screen blanks
 --dump          [<number>]        write vcsa<number> console dump to file
 --append        [<number>]        append vcsa<number> console dump to file
 --file          <filename>        name of the dump file
 --msg           [on|off]          send kernel messages to console
 --msglevel      0-8               kernel console log level
 --powersave     [on|vsync|hsync|powerdown|off]
                                   set vesa powersaving features
 --powerdown     [0-60]            set vesa powerdown interval in minutes
 --blength       [0-2000]          duration of the bell in milliseconds
 --bfreq         <number>          bell frequency in Hertz
 --version                         show version information and exit
 --help                            display this help and exit

For more details see setterm(1).

~~~
