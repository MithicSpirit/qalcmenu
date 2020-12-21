# menu-qalc
A calculator for Rofi/dmenu(2)

[Screencast](https://gfycat.com/SociableDopeyHerald)

## Installation
Arch Linux AUR: [menu-qalc](https://aur.archlinux.org/packages/menu-qalc/)

## Dependencies
- [bc](https://www.archlinux.org/packages/extra/x86_64/bc/)
- [xclip](https://www.archlinux.org/packages/extra/x86_64/xclip/)
- [Rofi](https://aur.archlinux.org/packages/rofi-git/) or
  dmenu[(2)](https://aur.archlinux.org/packages/dmenu2/)

## Usage
`menu-qalc` uses `qalc` as the backend and will accept any operations `qalc` is able to do:

    = 4+4
    = (4+2)/(4+3)
    = 4^2
    = sqrt(4)
    = c(2)
    = '1000 EUR to USD'

The answer can be copied to the clipboard and used for further calculations
inside (or outside) Rofi/dmenu.

If launched outside of Rofi/dmenu the expression may need quotation marks.

## Custom Usage
To launch directly into the calculator, use the following command (useful if
bound to "super + equal" in [sxhkd](https://github.com/baskerville/sxhkd),
[i3](https://i3wm.org/) or the like):

    = -- [rofi/dmenu parameters]

For example:

    = -- -location 2 -width 100

### Force usage of `dmenu`
By default, if `rofi` is installed, it will be used. You can force `menu-qalc`
to use `dmenu` or any other `dmenu`-like application:

    = --dmenu=dmenu
