# configuration-terminator

Terminator (like any other terminal emulator) is used by some extremely interactive console programs usually using ncurses or slang.
Keyboard assignments understood my Terminator are NOT available to the program which is reading keystrokes from the terminal.
Programs which execute in the terminal do not use menus or respond to the press of a modifier key (good).

Therefore, all typical control-key assignments (and all others) are assigned to alt-key.
Creating a new standard:
- Terminal Alt keys control the terminal itself.
- Terminal Ctrl keys are passed to the program using the terminal (see ncurses and slang).

The following keys are not part of preferences, but remain trapped (not passed on):
- Control-C (Cancel).
- Control-z (Suspend).
- Control-q (resume terminal).
- Control-s (stop terminal -- wait for resume (^q)).
