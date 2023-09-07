# configuration-terminator

Terminator (like any other terminal emulator) is used highly interactive consoole programs like mutt.
Keyboard assignments which are understood my Terminator are NOT available to the program which is reading keystrokes from the terminal.
Programs which execute in the terminal do not use menus or respond to the press of a modifier key (good).

Therefore, all typical control-key assignments (and all others) are assigned to alt-key.
Creating a new standard:
- Alt in the termial controls the terminal.
- Ctrl in the terminal are passed to the program using the terminal (see ncurses and slang).
