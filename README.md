# Based on Lukesmith'build and reformated on ubuntu systems

## FAQ

> What are the bindings?

This is suckless, mmmbud, the source code is the documentation! Check out [config.h](config.h).

## Patches and features

- Clickable statusbar with my build of [dwmblocks](https://github.com/muelthebest/dwmblocks).
- Reads xresources colors/variables (i.e. works with `pywal`, etc.).
- scratchpad: Accessible with mod+shift+enter.
- New layouts: bstack, fibonacci, deck, centered master and more. All bound to keys `super+(shift+)t/y/u/i`.
- True fullscreen (`super+f`) and prevents focus shifting.
- Windows can be made sticky (`super+s`).
- stacker: Move windows up the stack manually (`super-K/J`).
- shiftview: Cycle through tags (`super+g/;`).
- vanitygaps: Gaps allowed across all layouts.
- swallow patch: if a program run from a terminal would make it inoperable, it temporarily takes its place to save space.

## Installation for newbs

```
git clone https://github.com/muelthebest/dwm
cd dwm
sudo make install
```

## Please install `libxft-bgra`!

This build of dwm does not block color emoji in the status/info bar, so you must install [libxft-bgra](https://github.com/uditkarode/libxft-bgra) from the AUR, which fixes a libxft color emoji rendering problem, otherwise dwm will crash upon trying to render one. Hopefully this fix will be in all libxft soon enough.
See tutorial after remove default libxft ("this code remove association packages with libxft, warning!")

-            git clone https://github.com/uditkarode/libxft-bgra
-            cd libxft-bgra
-            sh autogen.sh --sysconfdir=/etc --prefix=/usr --mandir=/usr/share/man
-            sudo make install

>> Learn to how implement my system on [dotfiles](https://github.com/muelthebest/dotfiles)
