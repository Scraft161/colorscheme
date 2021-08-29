# colorscheme
home of Scraft, Scraft-dark, and Scraft-light

# About
Scraft is a colorscheme made for people who enjoy a simple colorscheme with dark backgrounds but still want full-tone colors

This colorscheme comes with 3 variants:

Scraft:
	The default colorscheme, comes with vibrant colors and dark backgrounds

Scraft-dark:
	Like the normal colorscheme, but offers darker colors

Scraft-light:
	Like the normal colorscheme, but is tweaked for light theme

# Colors

## Base
Background:	'#0a0a0a'
Foreground:	'#dddddd'

## 0-15
0:	'#0a0a0a'
1:	'#aa0a0a'
2:	'#0aaa0a'
3:	'#aaaa0a'
4:	'#0a0aaa'
5:	'#aa0aaa'
6:	'#0aaaaa'
7:	'#aaaaaa'

8:	'#222222'
9:	'#dd2222'
10:	'#22dd22'
11:	'#dddd22'
12: '#2222dd'
13:	'#dd22dd'
14:	'#22dddd'
15:	'#dddddd'

## Extended colors
16-255 shouldn't be allocated as of now

# Importing
You can use this colorscheme in various ways

## Xresources
The most used and universal way to set a colorscheme on your system.

```Xresources
! special
*.foreground:   #dddddd
*.background:   #0a0a0a
*.cursorColor:  #dddddd

! black
*.color0:       #0a0a0a
*.color8:       #222222

! red
*.color1:       #aa0a0a
*.color9:       #dd2222

! green
*.color2:       #0aaa0a
*.color10:      #22dd22

! yellow
*.color3:       #aaaa0a
*.color11:      #dddd22

! blue
*.color4:       #0a0aaa
*.color12:      #2222dd

! magenta
*.color5:       #aa0aaa
*.color13:      #dd22dd

! cyan
*.color6:       #0aaaaa
*.color14:      #22dddd

! white
*.color7:       #aaaaaa
*.color15:      #dddddd
```

## Alacritty
If you use alacritty as terminal emulator the best way to do this is:

1. Create a file `scraft.yml` in your alacritty config folder
2. Add the following to your `alacritty.yml`
```yml
import:
  - ${PATH-TO-CONF-DIR}/scraft.yml
```
3. Add the following to `scraft.yml`
```yml
colors:
  # Default colors
  primary:
    background: '0x0a0a0a'
    foreground: '0xdddddd'

  # Normal colors
  normal:
    black:   '0x0a0a0a'
    red:     '0xaa0a0a'
    green:   '0x0aaa0a'
    yellow:  '0xaaaa0a'
    blue:    '0x0a0aaa'
    magenta: '0xaa0aaa'
    cyan:    '0x0aaaaa'
    white:   '0xaaaaaa'

  # Bright colors
  bright:
    black:   '0x222222'
    red:     '0xdd2222'
    green:   '0x22dd22'
    yellow:  '0xdddd22'
    blue:    '0x2222dd'
    magenta: '0xdd22dd'
    cyan:    '0x22dddd'
    white:   '0xdddddd'
```
