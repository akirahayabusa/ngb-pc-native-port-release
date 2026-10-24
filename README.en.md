[简体中文](README.md) | **English**

# Ninja Gaiden Black Hurricane · native PC port

An unofficial native Windows port of Ninja Gaiden Black's Hurricane Chinese translation **vb-zh-x2.1** (original Xbox).

This repository only publishes the program; it holds no source code.

## Download

- [GitHub Releases](https://github.com/akirahayabusa/ngb-pc-native-port-release/releases): download `ngb-hurricane-pc-1.0.1-win32.zip`.
- Baidu Netdisk: <https://pan.baidu.com/s/1hZIwmm2hG-FY49zTiQROJw?pwd=ikwv>, code `ikwv`.
- Project site: <https://akirahayabusa.github.io/ngb-hurricane-patch/>

`-symbols.zip` holds debug symbols, needed only to report a crash.

## How it differs from the recompiled version

The x86 code in the original `default.xbe` runs unchanged on the PC's CPU. The Xbox's system parts (kernel, Direct3D, sound, controllers) are reimplemented on the PC by the loader.

- The game logic is the original code, so translating the code cannot add new bugs.
- Direct3D 9 is enough; integrated graphics run it at a full 60 fps.
- The arcade version and the SFC trilogy start from the main menu.
- Saves are in the standard Xbox format and can be exchanged with xRevive.
- Controllers: Xbox, PS3/4/5, Switch Pro, Joy-Con and DirectInput pads work directly, all with rumble.
- Optional Insignia online leaderboards.

## To play

1. Download the zip and extract it anywhere.
2. Open `NGB-Hurricane\Ninja Gaiden Black Hurricane Launcher.exe` and install your own vb-zh-x2.1 image (`.iso`) on the Install page.
3. Start from the Play page. Once installed, you can also double-click `Ninja Gaiden Black Hurricane.exe`.

**Requires**: Windows 10 / 11 and a Direct3D 9 graphics card (integrated graphics work); nothing else to install.

**The game is not included**: use your own legally obtained game image.

The full guide (settings, online play, known issues) is `README.en.md` in the zip.

## Legal

This project is not affiliated with or endorsed by Koei Tecmo, Team NINJA or Microsoft. Ninja Gaiden is a trademark of Koei Tecmo; Xbox is a trademark of Microsoft.

The program is licensed under the GNU General Public License, version 2 or (at your option) any later version; see `LICENSE`.

Developed by 哈雅布撒 (bilibili)
