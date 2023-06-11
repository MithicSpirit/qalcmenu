# qalcmenu
A qalc frontend for menus like rofi, bemenu, and dmenu. This is a fork of
[menu-qalc](https://github.com/barbuk/menu-qalc), but supporting Wayland instead
of X and with more robust command line arguments.

## Installation
Copy `=` into your `$PATH` and `qalcmenu.1` and `=.1` into your `$MANPATH`. On
most systems, running the following as root should suffice
```bash
install -m755 -t /usr/bin ./qalcmenu ./=
install -m644 -t /usr/share/man/man1 ./qalcmenu.1 ./=.1
```

## Dependencies
- [libqalculate](https://github.com/Qalculate/libqalculate)
- [xclip](https://github.com/bugaevc/wl-clipboard)
- A menu like [rofi](https://github.com/davatorium/rofi),
  [bemenu](https://github.com/Cloudef/bemenu),
  or [dmenu](https://tools.suckless.org/dmenu/)

## Usage
See `= --help` or `man qalcmenu.1`.

## License
This is based on code by (or licensed by) [@barbuk](https://github.com/BarbUk),
which is under an
[MIT License](https://github.com/BarbUk/menu-qalc/blob/80ae93f456a121faae86d7bb587e3696e93cff22/LICENSE).

As this is a major rewrite from the original code, maintaining only the idea, I
have relicensed it under AGPL-3.0. Please see the LICENSE file for more
information.
