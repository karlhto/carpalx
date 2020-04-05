# carpalx (QGMLWB)

## Description

This repo contains the carpalx layouts (will eventually support all of them, but only QGMLWB currently). `carpalx.xkb` contains a slightly modified version of the QGMLWB layout that ships with arch, with modifiers for `AltGr`, as well as Norwegian characters `Æ`, `Ø` and `Å` on `AltGr+A`, `AltGr+O` and `AltGr+E` respectively.

## Installation

Copy `carpalx.xkb` to your XKB symbols directory:

```bash
$ cp carpalx.xkb /usr/share/X11/xkb/symbols/carpalx
```

You should now be able to set the layout with:

```bash
$ setxkbmap carpalx
```
