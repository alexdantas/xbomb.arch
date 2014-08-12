# xbomb.arch

This repository contains the **Arch Linux packaging files** for the game xbomb
(_a version of the minesweeper game for X Windows_).

If you're after the game itself, [go to it's homepage][home].

![screen](http://www.gedanken.org.uk/software/xbomb/hexagon.png)

## Arch Linux packaging

* [**xbomb on AUR**][aur]

Unlike [other systems](https://github.com/alexdantas/xbomb.debian), packaging
for Arch Linux is fairly easy.

All you need is inside the file PKGBUILD.

## Getting Started

Here's a regular workflow...

```bash
# Retrieves the latest package files
$ git clone https://github.com/alexdantas/xbomb.arch
$ cd xbomb.arch

# Work on your changes...

# If the source file changed, this updates
# the PKGBUILD with new checksums
$ updpkgsums

# This command does the following:
# 1. Gets the source code;
# 2. Validates it with sha256sums;
# 3. Compiles it on the current dir;
$ makepkg

# Creates an AUR ball (.src.tar.gz), ready to
# be uploaded to AUR
$ mkaurball

# Nice helper that directly uploads to AUR
burp *.src.tar.gz
```

[home]: http://www.gedanken.org.uk/software/xbomb/
[aur]:  https://aur.archlinux.org/packages/xbomb/

