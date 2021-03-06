# uxterm command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


XTerm(327) usage:
    xterm [-options ...] [-e command args]

where options include:
    -/+132                       turn on/off 80/132 column switching
    -C                           intercept console messages
    -Sccn                        slave mode on "ttycc", file descriptor "n"
    -T string                    title name for window
    -/+ah                        turn on/off always highlight
    -/+ai                        turn off/on active icon
    -/+aw                        turn on/off auto wraparound
    -b number                    internal border in pixels
    -baudrate rate               set line-speed (default 38400)
    -/+bc                        turn on/off text cursor blinking
    -bcf milliseconds            time text cursor is off when blinking
    -bcn milliseconds            time text cursor is on when blinking
    -bd color                    border color
    -/+bdc                       turn off/on display of bold as color
    -bg color                    background color
    -bw number                   border width in pixels
    -/+cb                        turn on/off cut-to-beginning-of-line inhibit
    -cc classrange               specify additional character classes
    -/+cjk_width                 turn on/off legacy CJK width convention
    -class string                class string (XTerm)
    -/+cm                        turn off/on ANSI color mode
    -/+cn                        turn on/off cut newline inhibit
    -cr color                    text cursor color
    -/+cu                        turn on/off curses emulation
    -/+dc                        turn off/on dynamic color selection
    -display displayname         X server to contact
    -e command args ...          command to execute
    -fa pattern                  FreeType font-selection pattern
    -fb fontname                 bold text font
    -/+fbb                       turn on/off normal/bold font comparison inhibit
    -/+fbx                       turn off/on linedrawing characters
    -fd pattern                  FreeType Doublesize font-selection pattern
    -fg color                    foreground color
    -fi fontname                 icon font for active icon
    -fn fontname                 normal text font
    -fs size                     FreeType font-size
    -/+fullscreen                turn on/off fullscreen on startup
    -fw fontname                 doublewidth text font
    -fwb fontname                doublewidth bold text font
    -fx fontname                 XIM fontset
    %geom                        Tek window geometry
    #geom                        icon window geometry
    -geometry geom               size (in characters) and position
    -help                        print out this message
    -/+hm                        turn on/off selection-color override
    -/+hold                      turn on/off logic that retains window after exit
    -iconic                      start iconic
    -/+ie                        turn on/off initialization of 'erase' from pty
    -/+im                        use insert mode for TERMCAP
    -into windowId               use the window id given to -into as the parent window rather than the default root window
    -/+itc                       turn off/on display of italic as color
    -/+j                         turn on/off jump scroll
    -/+k8                        turn on/off C1-printable classification
    -kt keyboardtype             set keyboard type: tcap sun vt220
    -/+l                         turn on/off logging
    -/+lc                        turn on/off locale mode using luit
    -lcc path                    filename of locale converter (/usr/bin/luit)
    -leftbar                     force scrollbar left
    -lf filename                 logging filename
    -/+ls                        turn on/off login shell
    -/+maximized                 turn on/off maxmize on startup
    -/+mb                        turn on/off margin bell
    -mc milliseconds             multiclick time in milliseconds
    -/+mesg                      forbid/allow messages
    -/+mk_width                  turn on/off simple width convention
    -ms color                    pointer color
    -n string                    icon name for window
    -name string                 client instance, icon, and title strings
    -nb number                   margin bell in characters from right end
    -/+nul                       turn off/on display of underlining
    -/+pc                        turn on/off PC-style bold colors
    -/+pob                       turn on/off pop on bell
    -report-colors               report colors as they are allocated
    -report-fonts                report fonts as loaded to stdout
    -rightbar                    force scrollbar right (default left)
    -/+rv                        turn on/off reverse video
    -/+rvc                       turn off/on display of reverse as color
    -/+rw                        turn on/off reverse wraparound
    -/+s                         turn on/off multiscroll
    -/+samename                  turn on/off the no-flicker option for title and icon name
    -/+sb                        turn on/off scrollbar
    -selbg color                 selection background color
    -selfg color                 selection foreground color
    -/+sf                        turn on/off Sun Function Key escape codes
    -sh number                   scale line-height values by the given number
    -/+si                        turn on/off scroll-on-tty-output inhibit
    -/+sk                        turn on/off scroll-on-keypress
    -sl number                   number of scrolled lines to save
    -/+sm                        turn on/off the session-management support
    -/+sp                        turn on/off Sun/PC Function/Keypad mapping
    -/+t                         turn on/off Tek emulation window
    -ti termid                   terminal identifier
    -title string                title string
    -tm string                   terminal mode keywords and characters
    -tn name                     TERM environment variable name
    -/+u8                        turn on/off UTF-8 mode (implies wide-characters)
    -/+uc                        turn on/off underline cursor
    -/+ulc                       turn off/on display of underline as color
    -/+ulit                      turn off/on display of underline as italics
    -/+ut                        turn on/off utmp support
    -/+vb                        turn on/off visual bell
    -version                     print the version number
    -/+wc                        turn on/off wide-character mode
    -/+wf                        turn on/off wait for map before command exec
    -xrm resourcestring          additional resource specifications
    -ziconbeep percent           beep and flag icon of window having hidden output

Fonts should be fixed width and, if both normal and bold are specified, should
have the same size.  If only a normal font is specified, it will be used for
both normal and bold text (by doing overstriking).  The -e option, if given,
must appear at the end of the command line, otherwise the user's default shell
will be started.  Options that start with a plus sign (+) restore the default.


~~~
