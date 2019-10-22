
Debian
====================
This directory contains files used to package liracoind/liracoin-qt
for Debian-based Linux systems. If you compile liracoind/liracoin-qt yourself, there are some useful files here.

## liracoin: URI support ##


liracoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install liracoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your liracoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/liracoin128.png` to `/usr/share/pixmaps`

liracoin-qt.protocol (KDE)

