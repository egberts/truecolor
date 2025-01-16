# truecolor
A list of apps that can support TrueColor as well as ANSI, xterm, ESC, CSI, DSC, OSC, API, PM, STR, AKA, and some proprietary


Sources:

* TrueColor, central master repository - https://github.com/egberts/truecolor/blob/master/README.md
* A list of terminals, terminal emulators & console apps - https://github.com/cdleon/awesome-terminals
* VTE tester - https://www.invisible-island.net/vttest/
* Top Vim/NeoVim color scheme - https://vimcolorschemes.com/i/top
* `vim` command `:h xterm-true-color`

# `$COLORTERM` environment variable
`$COLORTERM` is a temporary environment variable name used by some certain terminal emulators (iTerm2, KiTTY)
used as a transitory path toward full true color.  Valid value of `$COLORTERM` is only `color`, `truecolor`, 
or blank.  `$COLORTERM` environment variable may even be undefined.

`$COLORTERM=truecolor` is the only way to expand from 256-color to 16M-color (but some will put `$COLORTERM=24bit` and this is not the norm, and should fell out of disuse).

# `$TERM` environment variable

It is no longer a good practice to set the `$TERM` environment variable.  `$TERM` get sets by the
terminal emulator, console, framebuffer driver, virtual pseudo-tty, SSH clients and certain apps (like email client,
chat, or network utilities).

The valid value for `$TERM` is entirely defined ONLY in the `/usr/share/terminfo/x` directory.

There is no `truecolor`-variant value for `$TERM`.  Maxes out at `TERM=xterm+256color`.
