# Native Ports

This is the **"Native-Ports.md"** file contains the best ports i suggest and how to install them.


## Prerequisites

### Shader Compiler (libshacccg)

The legal shader compiler **(libshaccg.suprx)** helps to make the developers, porters, or anyone who wants to make anything to PSVita easily to develop, ports a game or app to PSVita. 

1. Download and install this app called **[PIB-Configuration-Tool](https://github.com/ZHassanQ/Vita-Guide/releases/download/VPK/PIBConfig.vpk)** to your PSVita. (Developed by **[SonicMastr](https://github.com/SonicMastr/)**)
2. Launch and press the Select button.

### Plugins

And also you to play these ports you will need these **[plugin](https://github.com/TheOfficialFloW/kubridge)-[s.](https://github.com/TheOfficialFloW/FdFix)** As said from the official porters. (These plugins **aren't** included in AIO pack)

1. Copy **[kubridge.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/kubridge.skprx)** to `ur0:tai` folder, add **"kubridge.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[fd_fix.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/fd_fix.skprx)** to `ur0:tai` folder, add **"fd_fix.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
- **"fd_fix.skprx"** plugin isn't required if you installed **"repatch"** plugin.

### Installed

```

• KERNEL

ur0:tai/kubridge.skprx
ur0:tai/fd_fix.skprx

```

## Optional

If you want more performance then use these two plugins: (These plugins **are** included in AIO pack) 

- **[NoCapUnlocker](https://github.com/GrapheneCt/CapUnlocker)** Unlocks some non-game capabilities for PS Vita homebrew apps. (**[Guide](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-5-capunlocker)**)
- **[PSVshell](https://github.com/Electry/PSVshell)** Yet another overclocking plugin. Use it to overclock your PSVita to 500Mhz. (**[Guide](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-6-psvshellplus)**)


# TheOfficialFlow Ports

**[TheOfficialFlow](https://github.com/TheOfficialFloW)** ports uses the android version of the game's which uses ARMv7 and recall it syscalls so that the PSVita can provide what the game wants with **[vitaGL.](https://github.com/TheOfficialFloW/vitaGL)** (OpenGL for PSVita)

## Bully: Anniversary Edition

**[Bully: Anniversary Edition](https://github.com/TheOfficialFloW/bully_vita)** port uses **any version** of the game's APK.

## Crazy Taxi: Classic

**[Crazy Taxi: Classic](https://github.com/TheOfficialFloW/crazytaxi_vita)** port uses **any version** of the game's APK.

## Grand Theft Auto: Chinatown Wars

**[Grand Theft Auto: Chinatown Wars](https://github.com/TheOfficialFloW/gtactw_vita)** port uses **1.04 version** of the game's APK.

## Grand Theft Auto: San Andreas

**[Grand Theft Auto: San Andreas](https://github.com/TheOfficialFloW/gtasa_vita)** port uses **2.00 version** of the game's APK.



# SonicMastr Ports

**[SonicMastr](https://github.com/SonicMastr/)** as his name ports Sonic games for now he ported: Sonic 1, 2, CD, & Mania. All of his ports requires the assets of the original game which can be obtained from legaly purchased APK or a Steam version.

## Sonic 1, 2

**[Sonic-1-2](https://github.com/SonicMastr/Sonic-1-2-Vita/releases)** port forks from Sonic 1, 2 **[Decompilation](https://github.com/Rubberduckycooly/Sonic-1-2-2013-Decompilation)** version of it. (Only **APK** version is supported)

## Sonic CD

**[Sonic-CD](https://github.com/SonicMastr/Sonic-CD-Vita/releases)** port forks from Sonic CD **[Decompilation](https://github.com/Rubberduckycooly/Sonic-CD-11-Decompilation)** version of it. (**APK** and **Steam** version are supported)

## Sonic Mania

**[Sonic-Mania](https://github.com/SonicMastr/Sonic-Mania-Vita)** port forks from Sonic CD **[Decompilation](https://github.com/Rubberduckycooly/Sonic-Mania-Decompilation)** version of it. (**Steam, Epic Games, & Origins** version are supported)



# Others
## Super Mario Bros

This **[Super Mario Bros](https://github.com/WeegeeDEVELOPER/uMario-PSVita-Port)** port has been ported from **[WeegeeDEVOLPER](https://github.com/WeegeeDEVELOPER/)** using this **[repository](https://github.com/jakowskidev/uMario_Jakowski)** which is a C++ version of the game developed by **[uMario_Jakowski.](https://github.com/jakowskidev/uMario_Jakowski)**

### Installation

1. Simply install this **[VPK file](https://github.com/ZHassanQ/Vita-CFW-Guide/releases/download/Assets/uMario_v1.2.7.vpk)** as it isn't illegal as it doesn't contain any original assets from the NES game.

## Super Mario 64

This **[Super Mario 64](https://github.com/martepato/sm64-vita)** port has been ported from **[bythos](https://github.com/bythos14/)** using this **[repository](https://github.com/sm64-port/sm64-port)** that contains a full decompilation of Super Mario 64 (J), (U), (E), and (SH). Then **[martepato](https://github.com/martepato/)** enhanced it.

### Installation

1. Download the **[master branch]()** of this **[repository.](https://github.com/martepato/sm64-vita)** (**"master branch"** links to a backup in this repository)
2. Download and install **[VitaSDK](https://vitasdk.org/)**
3. Enter the **"masteer branch"** by Terminal, CMD. `cd sm64-vita`
4. Place a Super Mario 64 ROM called **"baserom.<VERSION>.z64"** into the repository's root directory for asset extraction, where **"VERSION"** can be `us`, `jp`, or `eu`
5. Run these commands: `./build_deps.sh`, `make TARGET_VITA=1 vpk`
6. The installable VPK file will be found in `sm64-vita-master/build/<VERSION>_vita`

## Max Payne

This **[Max Payne](https://github.com/fgsfdsfgs/max_vita)** port has been ported from **[fgsfdsfgs](https://github.com/fgsfdsfgs/)** and it uses a legally purchased APK 1.7 version of Max Payne. (This port mostly uses TheOfficialFlow ports way)

### Installation

1. Create a directory in `ux0:data/` folder, call it **"maxpayne"**
2. Extract **"assets"** folder from your APK to `ux0:data/maxpayne` folder.
3. Extract **"libMaxPayne.so"** file from your APK in `lib/armeabi-v7a` folder to `ux0:data/maxpayne` folder.
4. Extract **".obb"** file from your APK to `ux0:data/maxpayne` folder.
5. Extract **[data.zip](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/MaxPayne-data.zip)** to `ux0:data` folder.
6. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/MaxPayne_r4.vpk)** (It will create a shortcut in live area) 

### Notes

The Vita port has an extra config file, located at `ux0:/data/maxpayne/config.txt` It is created when you first run the game and allows you to tweak some internal settings. For more detailed descriptions of said settings check the **[wiki article.](https://github.com/fgsfdsfgs/max_vita/wiki/Config-variables)**

- If the error says Could not find symbol, that likely means you have the wrong APK version. You need one for v1.7, others will not work.
