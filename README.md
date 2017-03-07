## menu-calc
A calculator for Rofi/dmenu(2)  
[Screencast](https://gfycat.com/SociableDopeyHerald)

## Dependencies
[bc](https://www.archlinux.org/packages/extra/x86_64/bc/)  
[xclip](https://www.archlinux.org/packages/extra/x86_64/xclip/)  
[Rofi](https://aur.archlinux.org/packages/rofi-git/) or dmenu[(2)](https://aur.archlinux.org/packages/dmenu2/)

## Usage
`menu-calc` uses `bc` as the backend and will accept any operations `bc` is able to do:
```
= -h
= 4+4
= (4+2)/(4+3)
= 4^2
= sqrt(4)
= c(2)`
```

The answer can be copied to the clipboard and used for further calculations inside (or outside) Rofi/dmenu.

If launched outside of Rofi/dmenu the expression may need quotation marks.

## Custom Usage
To launch directly into the calculator, use the following command (useful if bound to "super + equal" in [sxhkd](https://github.com/baskerville/sxhkd) or the like):
```
=
```
