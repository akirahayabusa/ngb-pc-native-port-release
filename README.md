**简体中文** | [English](README.en.md)

# 忍者龙剑传 黑之章 · PC 原生移植

《忍者龙剑传 黑之章》（初代 Xbox）的非官方 Windows 原生移植。支持这四种光盘镜像：

- 美版原版 NINJA GAIDEN BLACK（英文）
- 基本版 va-zh-x2（中英）
- 飓风版 vb-zh-x2.1（中英）
- 飓风版 vb-jp-x2.1（日英）

这个仓库只用来发布程序，不含源码。

## 下载

- [GitHub Releases](https://github.com/akirahayabusa/ngb-pc-native-port-release/releases)：下载 `ngb-hurricane-pc-1.2.0-win32.zip`。
- 夸克网盘：<https://pan.quark.cn/s/c210df004321>。
- 项目主页：<https://akirahayabusa.github.io/ngb-hurricane-patch/>

`-symbols.zip` 是调试符号，只在回报崩溃时需要。

## 和重编译版有什么不同

原版 `default.xbe` 里的 x86 代码一条不改，直接在 PC 的 CPU 上运行。Xbox 的内核、Direct3D、声音、手柄这些系统部分，由加载器在 PC 上重新实现。

- 游戏逻辑就是原版那份代码，不会因为翻译代码产生新 bug。
- 只需要 Direct3D 9，集成显卡也能跑满 60 帧。
- 街机版（飓风版还有 SFC 三部曲）都能从主菜单进入。
- 存档是标准 Xbox 格式，可以和 xRevive 互导。
- 手柄：Xbox、PS3/4/5、Switch Pro、Joy-Con、DirectInput 手柄都能直接用，都带震动。
- 可选的 Insignia 联网排行榜。

## 怎么玩

1. 下载压缩包，解压到任意位置。
2. 打开 `NGB-Hurricane\Ninja Gaiden Black Any Launcher.exe`，在「安装」页选择你自己的游戏镜像（`.iso`，上面四种之一）安装。
3. 回到「开始游戏」页开始。装好后也可以直接双击 `Ninja Gaiden Black Any.exe`。

从 1.1.12 或更早的版本升级：1.2.0 起程序改名为 `Ninja Gaiden Black Any.exe` / `Ninja Gaiden Black Any Launcher.exe`，覆盖解压后可以删掉旧的 `Ninja Gaiden Black Hurricane.exe` 和 `Ninja Gaiden Black Hurricane Launcher.exe`，桌面快捷方式要重新建。存档和设置不受影响。

**需要**：Windows 10 / 11，支持 Direct3D 9 的显卡（集成显卡也可以），不用装任何运行库。

**不包含游戏本身**：请使用你自己合法取得的游戏镜像。

完整说明（设定、联网、已知问题）见压缩包里的 `README.md`。

## 法律声明

本项目与 Koei Tecmo、Team NINJA 及 Microsoft 无关，也未获其认可。Ninja Gaiden 是 Koei Tecmo 的商标，Xbox 是 Microsoft 的商标。

程序以 GNU 通用公共许可证第 2 版或（由你选择）任何更新的版本发布，见 `LICENSE`。

开发：哈雅布撒（b 站）
