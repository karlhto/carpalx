# carpalx
## Description
The carpalx layouts for Linux. This is a slightly modified version of 
[this layout](www.khjk.org/log/2011/jan/carpalx.html). It adds correct
modifiers for `AltGr`, as well as Norwegian characters `Æ`, `Ø` and `Æ` on
`AltGr+A`, `AltGr+O` and `AltGr+E` respectively.

## Installation
Copy `carpalx.xkb` to your XKB symbols directory:

```bash
$ cp carpalx.xkb /usr/share/X11/xkb/symbols/carpalx
```

and add the following lines to `/usr/share/X11/xkb/symbols.dir`:

```
-dp----- a------- carpalx(qgmlwb)
--p----- a------- carpalx(qgmlwy)
--p----- a------- carpalx(qfmlwy)
--p----- a------- carpalx(qwkrfy)
--p----- a------- carpalx(qwyrfm)
--p----- a------- carpalx(tnwmlc)
```

You should now be able to set the layout with:

```bash
$ setxkbmap carpalx                          # defaults to qgmlwb
$ setxkbmap -layout carpalx -variant qgmlwy  # to select a variant
```
