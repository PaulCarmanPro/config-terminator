# configuration-terminator

Terminator (like any other terminal emulator) is used by some extremely interactive console programs usually using ncurses or slang.
Keyboard assignments understood my Terminator are NOT available to the program which is reading keystrokes from the terminal.
Programs which execute in the terminal lack menus, buttons, and the ability to respond to the press of a modifier key alone.

All typical control-key assignments (and all others) are assigned to alternate key.
This creates a new standard which previously was Shift-Control:
- Terminal Alt keys control the terminal itself.
- Terminal Ctrl keys are passed to the program using the terminal (see ncurses and slang).

Note: Mutt doesnot sees Shift-Ctrl as Ctrl and doesnot see Alt at all.

The following keys are not part of preferences, but often remain trapped (not passed on):
- Control-C (Cancel).
- Control-z (Suspend).
- Control-q (resume terminal).
- Control-s (stop terminal -- wait for resume (^q)).
