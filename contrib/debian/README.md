
Debian
====================
This directory contains files used to package voltaemd/voltaem-qt
for Debian-based Linux systems. If you compile voltaemd/voltaem-qt yourself, there are some useful files here.

## voltaem: URI support ##


voltaem-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install voltaem-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your voltaem-qt binary to `/usr/bin`
and the `../../share/pixmaps/voltaem128.png` to `/usr/share/pixmaps`

voltaem-qt.protocol (KDE)

