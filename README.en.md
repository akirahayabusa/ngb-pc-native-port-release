[简体中文](README.md) | **English**

# Ninja Gaiden Black · native PC port

An unofficial native Windows port of Ninja Gaiden Black (original Xbox). Four disc images are supported:

- the original US release NINJA GAIDEN BLACK (English)
- the basic edition va-zh-x2 (Chinese / English)
- the Hurricane edition vb-zh-x2.1 (Chinese / English)
- the Hurricane edition vb-jp-x2.1 (Japanese / English)

This repository only publishes the program; it holds no source code.

## Download

- [GitHub Releases](https://github.com/akirahayabusa/ngb-pc-native-port-release/releases): download `ngb-hurricane-pc-1.2.0-win32.zip`.
- Quark Netdisk: <https://pan.quark.cn/s/c210df004321>.
- Project site: <https://akirahayabusa.github.io/ngb-hurricane-patch/>

`-symbols.zip` holds debug symbols, needed only to report a crash.

## How it differs from the recompiled version

The x86 code in the original `default.xbe` runs unchanged on the PC's CPU. The Xbox's system parts (kernel, Direct3D, sound, controllers) are reimplemented on the PC by the loader.

- The game logic is the original code, so translating the code cannot add new bugs.
- Direct3D 9 is enough; integrated graphics run it at a full 60 fps.
- The arcade version (and, in the Hurricane editions, the SFC trilogy) start from the main menu.
- Saves are in the standard Xbox format and can be exchanged with xRevive.
- Controllers: Xbox, PS3/4/5, Switch Pro, Joy-Con and DirectInput pads work directly, all with rumble.
- Optional Insignia online leaderboards.

## To play

1. Download the zip and extract it anywhere.
2. Open `NGB-Hurricane\Ninja Gaiden Black Any Launcher.exe` and install your own game image (`.iso`, one of the four above) on the Install page.
3. Start from the Play page. Once installed, you can also double-click `Ninja Gaiden Black Any.exe`.

Upgrading from 1.1.12 or earlier: from 1.2.0 the programs are `Ninja Gaiden Black Any.exe` / `Ninja Gaiden Black Any Launcher.exe`. After extracting over the old folder you can delete the old `Ninja Gaiden Black Hurricane.exe` and `Ninja Gaiden Black Hurricane Launcher.exe`, and make desktop shortcuts again. Saves and settings are kept.

**Requires**: Windows 10 / 11 and a Direct3D 9 graphics card (integrated graphics work); nothing else to install.

**The game is not included**: use your own legally obtained game image.

The full guide (settings, online play, known issues) is `README.en.md` in the zip.

## Legal

This project is not affiliated with or endorsed by Koei Tecmo, Team NINJA or Microsoft. Ninja Gaiden is a trademark of Koei Tecmo; Xbox is a trademark of Microsoft.

The program is licensed under the GNU General Public License, version 2 or (at your option) any later version; see `LICENSE`.

Developed by 哈雅布撒 (bilibili)
