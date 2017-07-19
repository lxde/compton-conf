# compton-conf

## Overview

compton-conf is a configuration tool for X composite manager [Compton](https://github.com/chjj/compton).   

![Screenshot of compton-conf running on awesome-wm](http://i.imgur.com/2fSiAx8.png)

It is maintained by the LXQt project but can be used independently from this desktop environment.   

## Installation

### Compiling source code

Runtime dependencies are libconfig and qtbase.   
Additional build dependencies are CMake and [liblxqt](https://github.com/lxde/liblxqt) as well as optionally Git to pull latest VCS checkouts. The localization files were outsourced to repository [lxqt-l10n](https://github.com/lxde/lxqt-l10n) so the corresponding dependencies are needed, too. Please refer to this repository's `README.md` for further information.   

Code configuration is handled by CMake. CMake variable `CMAKE_INSTALL_PREFIX` has to be set to `/usr` on most operating systems.   

To build run `make`, to install `make install` which accepts variable `DESTDIR` as usual.   

### Binary packages

Official binary packages are available in Arch Linux, Debian (as of Debian stretch) and openSUSE (Leap 42.1 and Tumbleweed).   
The tool is missing in Fedora so far due to incomplete dependency listing and fedora naming conventions to identify fedora dependencies, in addition a large amount of qt packages generally installed separately from the qt libraries.
