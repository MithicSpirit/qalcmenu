# menu-qalc
A qalc frontend for menus like rofi, bemenu, and dmenu. This is a fork of
[menu-qalc](https://github.com/barbuk/menu-qalc), but supporting Wayland instead
of X and with more robust command line arguments.

## Installation
Copy `=` into your `$PATH` and `menu-qalc.1` and `=.1` into your `$MANPATH`. On
most systems, running the following as root should suffice
```bash
install -m755 ./= /usr/bin/=
install -m644 -t /usr/share/man/man1 ./=.1 ./menu-qalc.1
```

## Dependencies
- [libqalculate](https://github.com/Qalculate/libqalculate)
- [xclip](https://github.com/bugaevc/wl-clipboard)
- A menu like [rofi](https://github.com/davatorium/rofi),
  [bemenu](https://github.com/Cloudef/bemenu),
  or [dmenu](https://tools.suckless.org/dmenu/)

## Usage
See `= --help` or `man menu-qalc.1`.
