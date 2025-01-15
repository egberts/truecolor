# truecolor
A list of apps that can support TrueColor as well as ANSI, xterm, ESC, CSI, DSC, OSC, API, PM, STR, AKA, and some proprietary


Sources:

* TrueColor, central master repository - https://github.com/egberts/truecolor/blob/master/README.md
* A list of terminals, terminal emulators & console apps - https://github.com/cdleon/awesome-terminals
* VTE tester - https://www.invisible-island.net/vttest/
* Top Vim/NeoVim color scheme - https://vimcolorschemes.com/i/top

# $TERM environment variable

It is no longer a good practice to set the `$TERM` environment variable.  `$TERM` get sets by the
terminal emulator, console, framebuffer driver, virtual pseudo-tty, SSH clients and certain apps (like email client,
chat, or network utilities).

The valid value for `$TERM` is given ONLY in the `/usr/share/terminfo/x` directory.

There is no `truecolor`-variant for `$TERM`.  Maxed out at `TERM=xterm-256`.
