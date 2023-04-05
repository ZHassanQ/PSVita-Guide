# Native Ports

This is the **"Native-Ports.md"** file contains the best ports i suggest and how to install them. 


🧭 Table of Contents
 - 🔧 Devolopers
   - **[TheOfficialFlow](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-theofficialflow-ports)**
   - **[SonicMastr](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-sonicmastr-ports)**
   - **[Northfear](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-northfear-ports)**
   - **[Others](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-others)**
 - 👾 APK
   - **[Bully: Anniversary Edition](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-bully-anniversary-edition)**
   - **[Crazy Taxi: Classic](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-crazy-taxi-classic)**
   - **[Grand Theft Auto: Chinatown Wars](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-grand-theft-auto-chinatown-wars)**
   - **[Grand Theft Auto: San Andreas](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-grand-theft-auto-san-andreas)**
   - **[Sonic 1, 2, & CD](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-sonic-1-2--CD)**
   - **[Sonic Mania](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#%EF%B8%8F--sonic-mania)**
   - **[Max Payne](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-max-payne)**
 - 🖥️ Computer
   - **[Sonic Mania](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#%EF%B8%8F--sonic-mania)**
   - **[Fallout](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#%EF%B8%8F-fallout)**
   - **[Fallout 2](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#%EF%B8%8F-fallout-2)**
 - 🖱 Console Dump
   - **[Super Mario 64](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-super-mario-64)**
 - ☢️ No Copy Required
   - **[Super Mario Bros](https://github.com/ZHassanQ/Vita-Guide/blob/main/Native-Ports.md#-super-mario-bros)**

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


# 🔧 TheOfficialFlow Ports

**[TheOfficialFlow](https://github.com/TheOfficialFloW)** ports uses the android version of the game's which uses ARMv7 and recall it syscalls so that the PSVita can provide what the game wants with **[vitaGL.](https://github.com/TheOfficialFloW/vitaGL)** (OpenGL for PSVita)


## 👾 Bully: Anniversary Edition

**[Bully: Anniversary Edition](https://github.com/TheOfficialFloW/bully_vita)** port uses **any version** of the game's APK.

### Installation

1. Extract from game's APK: `Assets` folder contents, and `libarmeabi-v7a/libBully.so` file to `ux0:data/Bully` folder. 
2. Extract from game's APK: `Android/obb/com.rockstargames.bully/main.11.com.rockstargames.bully.obb` file, and `Android/obb/com.rockstargames.bully/patch.11.com.rockstargames.bully.obb` file to `ux0:data/Bully/Android` folder.
3. Rename **"main.11.com.rockstargames.bully.obb"** to **"main.obb"**
4. Rename **"patch.11.com.rockstargames.bully.obb"** to **"patch.obb"**
5. Extract **[data.zip](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Bully-data.zip)** to `ux0:data/Bully` folder.
6. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Bully_r1.vpk)** (It will create a shortcut in LiveArea) 

### Notes

- The official game does not free unused textures (as modern smartphones have more RAM than the PS Vita) and as such, the game will crash after a long gameplay.

## 👾 Crazy Taxi: Classic

**[Crazy Taxi: Classic](https://github.com/TheOfficialFloW/crazytaxi_vita)** port uses **any version** of the game's APK.

### Installation

1. Extract from game's APK: `Assets` folder contents, and `libarmeabi-v7a/libgl2jni.so` file to `ux0:data/crazytaxi` folder. 
2. Extract from game's APK: `Android/obb/com.sega.CrazyTaxi/main.67.com.sega.CrazyTaxi.obb` file to `ux0:data/crazytaxi
3. Rename **"main.67.com.sega.CrazyTaxi.obb"** to **"main.obb"**
4. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/CRAZYTAXI_r3.vpk)** (It will create a shortcut in LiveArea)

## 👾 Grand Theft Auto: Chinatown Wars

**[Grand Theft Auto: Chinatown Wars](https://github.com/TheOfficialFloW/gtactw_vita)** port uses **1.04 version** of the game's APK.

### Installation

1. Extract from game's APK: `Assets` folder contents, and `libarmeabi-v7a/libCTW.so` file to `ux0:data/gtactw` folder. 
2. Extract from game's APK: `Android/obb/com.rockstargames.gtactw/main.4.com.rockstargames.gtactw.obb` file on your Computer.
3. Extract **"main.4.com.rockstargames.gtactw.obb"** file contents to `ux0:data/gtactw` folder
4. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTACTW_r3.vpk)** (It will create a shortcut in LiveArea) 

## 👾 Grand Theft Auto: San Andreas

**[Grand Theft Auto: San Andreas](https://github.com/TheOfficialFloW/gtasa_vita)** port uses **2.00 version** of the game's APK.

### Installation

1. Extract from game's APK: `Assets` folder contents, and `libarmeabi-v7a/libGTASA.so` file to `ux0:data/gtasa` folder. 
2. Extract from game's APK: `Android/obb/com.rockstargames.gtasa/main.8.com.rockstargames.gtasa.obb` file, and `Android/obb/com.rockstargames.gtasa/patch.8.com.rockstargames.gtasa.obb` file on your Computer.
3. Extract **"main.8.com.rockstargames.gtasa.obb"** and **"patch.8.com.rockstargames.gtasa.obb"** files contents to `ux0:data/gtasa`
4. Extract **[data.zip](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTASA-data.zip)** to `ux0:data/gtasa` folder.
5. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTASA_r12.vpk)** (It will create a shortcut in LiveArea)

### PGTeam Mod

**[PGTeam](https://pgtmp.gitbook.io/pgbook_eng/)** have made mods to experience **Grand Theft Auto: San Andreas** as if it was the Defenitive Edition.

1. Delete **"cache"** folder from `ux0:data/gtasa` folder. (If found)
2. Extract **[GTASA-Mod.zip](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTASA-Mod.zip)** to `ux0:data/gtasa` folder. (Overwrite any file if requested)
3. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTASA_v2.1_PCAE.vpk)** over the one you installed.

### Notes

1. After fully installing the port, you'll be able to configure it with the Configurator app. The Configurator app will allow users to enable or disable a set of optimizations, patches and renderer alterations to best match users taste. You can launch the Configurator app by clicking on the Configuration button located on the LiveArea section.

2. In order to reduce occasional stutters in-game, delete both `ux0:data/gtasa/scache_small_low.txt` file and `ux0:data/gtasa/scache_small.txt` file, then create a copy of the `ux0:data/gtasa/scache.txt` file to have two version of it. (for example **"scache(1).txt"** so in the end you end up with both **"scache.txt"** and **"scache(1).txt"** inside the `ux0:data/gtasa/` folder), then rename **"scache.txt"** to **"scache_small.txt"** and "**scache(1).txt"** to **"scache_small_low.txt"** . This will however make the loading screen longer since it needs to compile more shaders ahead.
- If the folder `ux0:data/gtasa/cache` contains much more than 300 files, it's recommended to delete the folder and have it rebuilt.
3. You can input PC cheats by pressing L + SELECT to open the on-screen keyboard. See **[CHEATS.md](https://github.com/TheOfficialFloW/gtasa_vita/blob/master/CHEATS.md)** for available and unavailable cheats (you can input cheat codes in lowercase as well as uppercase).
- The L2/R2 buttons are mapped to the rear touchpad on the top and the L3/R3 buttons are mapped to the front touchpad on the bottom. With v1.2 and higher, you can map L2/R2 to the front touchpad on the top.
- You can open the map by holding START and then releasing.
- You can get local freeroam coop and rampages working by replacing the main scripts with those of the PS3 version. See **[COOP.md.](https://github.com/TheOfficialFloW/gtasa_vita/blob/master/COOP.md)**
- Due to expired licensing, some songs were cut from the game. See **[MUSIC.md](https://github.com/TheOfficialFloW/gtasa_vita/blob/master/MUSIC..md)** for a list of removed tracks and a guide on how to restore them.
- To properly take off during Learning to Fly mission, retract your landing gear by pressing RIGHT.


## Grand Theft Auto: Vice City, III

I can't provide any instructions on how to install either Vice City or III as their ports were decomplation of the PlayStation 2 version that was considered illegal by Take-Two Interactive company. And the original source was taken down due to DMCA. I can only provide mods that enhances the graphics and the look of the game to experience the game as if it was the Definitive Edition. The mods were made by **[PGTeam.](https://pgtmp.gitbook.io/pgbook_eng/)** This **[reddit post](https://www.reddit.com/r/VitaPiracy/comments/10j2erj/latest_backups_of_re3vita_14_revcvita_11_and/)** might help.

1. Grand Theft Auto: III
    - **[Mod](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTAIII-Mod.zip)**
    - **[VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTAIII_v1.4_PCAE.vpk)**
2. Grand Theft Auto: Vice City
    - **[Mod](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTAVC-Mod.zip)**
    - **[VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/GTAVC_v1.1_PCAE.vpk)**

# 🔧 SonicMastr Ports

**[SonicMastr](https://github.com/SonicMastr/)** as his name ports Sonic games for now he ported: Sonic 1, 2, CD, & Mania. All of his ports requires the assets of the original game which can be obtained from legaly purchased APK or a Steam version.

## 👾 Sonic 1, 2, & CD

- **[Sonic-1-2](https://github.com/SonicMastr/Sonic-1-2-Vita/releases)** port forks from Sonic 1, 2 **[Decompilation](https://github.com/Rubberduckycooly/Sonic-1-2-2013-Decompilation)** version of it. (Only **APK** version is supported)
- **[Sonic-CD](https://github.com/SonicMastr/Sonic-CD-Vita/releases)** port forks from Sonic CD **[Decompilation](https://github.com/Rubberduckycooly/Sonic-CD-11-Decompilation)** version of it. (Only **APK** version is supported)


### Installation

1. Place **"Data.rsdk.msf"** in `x0:data/Sonic1/` for Sonic the Hedgehog 1. 
2. Place **"Data.rsdk.msf"** in `ux0:data/Sonic2/` for Sonic the Hedgehog 2.
3. Place **"Data.rsdk.msf"** in `ux0:data/Sonic2/` for Sonic CD.
4. Rename all files to: **"Data.rsdk"**
5. Install **[Sonic1 VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Sonic1_r4.vpk)** file for Sonic the Hedgehog 1.
6. Install **[Sonic2 VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Sonic2_r4.vpk)** file for Sonic the Hedgehog 2.
7. Install **[SonicCD VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/SonicCD_r3.vpk)** file for Sonic CD.

### Notes

- Sonic 1, 2
  - Sounds stops working after suspension on some systems. It will start playing again after an event triggers playback.

- Sonic CD
  - Rare crash while loading a save or starting new game. Just restart.
  - Special Stages Run at around 40fps average. This is simply due to the Software renderer and should be fixed when a Hardware renderer is added.
  - A single frame flashes in-between transitions.


## 🖥️ 👾 Sonic Mania

**[Sonic-Mania](https://github.com/SonicMastr/Sonic-Mania-Vita)** port forks from Sonic CD **[Decompilation](https://github.com/Rubberduckycooly/Sonic-Mania-Decompilation)** version of it. (**Steam, Epic Games, & Origins** version are supported)

### Installation

1. Place **"Data.rsdk"** file (Can be obtained by buying the game) in `ux0:data/Mania`
2. Download these two **[Game.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Game.suprx)** - **[Settings.ini](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/Settings.ini)** files and put them in `ux0:data/Mania` folder.
3. Download this **[modconfig.ini](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/modconfig.ini)** file and put it in `ux0:data/Mania/mods` folder.
4. Install **[SonicMania VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/SonicMania_r3.vpk)** file.

### Notes

- Special stages are still slow. Still too slow. Very, very, veryyyy slow.
  - This **[mod](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/SonicMania-NoSSDecorations.zip)** (**[Original Source](https://gamebanana.com/mods/408483)**) remove some assets from special stages to load. it will help improving the performance.
- You can use mods by putting them in `ux0:data/Mania/mods/` folder.
  - Any mods that use a **".dll"** file will NOT work.
  - Asset/Palette swap mods will most likely require checking for `TargetVersion` to equal 5. MAKE SURE THIS IS CHECKED
- These two mods: **[MaxControlVita](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/MaxControlVita.zip)** and **[UltraWideManiaVita](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/UltrawideManiaVita.zip)** are from **[SonicMastr.](https://github.com/SonicMastr/)**


# Northfear Ports

**[Northfear](https://github.com/Northfear)** ports uses some assets from the game's CE (Community Edition) and the original game. (Can be obtained by purchasing the game)

## 🖥️ Fallout

**[Fallout](https://github.com/Northfear/fallout1-ce-vita)** port uses this **[Community Edition](https://github.com/alexbatalov/fallout1-ce)** and the original game to be played.

### Installation

1. Place **"MASTER.DAT"**, **"CRITTER.DAT"** files and **"DATA"** folder (Can be obtained by buying the game) in `ux0:data/fallout`
- Copy **"fallout.cfg"** too, if you're using non-english Fallout version.
  - Or make sure that language setting is properly set in it like: `language=german`
2. Install **[Fallout VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/fallout-ce_r2.vpk)** file.

## 🖥️ Fallout 2

**[Fallout 2](https://github.com/Northfear/fallout2-ce-vita)** port uses this **[Community Edition](https://github.com/alexbatalov/fallout2-ce)** and the original game to be played. 

1. Place **"master.dat"**, **"critter.dat"**, **"patch000.dat"** files, **"data"**, and **"sound"** folders (Can be obtained by buying the game) in `ux0:data/fallout2`
- Copy **"fallout2.cfg"** too, if you're using non-english Fallout version.
  - Or make sure that language setting is properly set in it like: `language=german`
2. Install **[Fallout 2 VPK](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/fallout2-ce_r10.vpk)** file.

# 🔧 Others
## ☢️ Super Mario Bros

This **[Super Mario Bros](https://github.com/WeegeeDEVELOPER/uMario-PSVita-Port)** port has been ported from **[WeegeeDEVOLPER](https://github.com/WeegeeDEVELOPER/)** using this **[repository](https://github.com/jakowskidev/uMario_Jakowski)** which is a C++ version of the game developed by **[uMario_Jakowski.](https://github.com/jakowskidev/uMario_Jakowski)**

### Installation

1. Simply install this **[VPK file](https://github.com/ZHassanQ/Vita-CFW-Guide/releases/download/Assets/uMario_v1.2.7.vpk)** as it isn't illegal as it doesn't contain any original assets from the NES game.

## 🖱 Super Mario 64

This **[Super Mario 64](https://github.com/martepato/sm64-vita)** port has been ported from **[bythos](https://github.com/bythos14/)** using this **[repository](https://github.com/sm64-port/sm64-port)** that contains a full decompilation of Super Mario 64 (J), (U), (E), and (SH). Then **[martepato](https://github.com/martepato/)** enhanced it.

### Installation

1. Download the **[master branch](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/sm64-vita-master.zip)** of this **[repository.](https://github.com/martepato/sm64-vita)** (**"master branch"** links to a backup in this repository)
2. Download and install **[VitaSDK](https://vitasdk.org/)**
3. Enter the **"master branch"** by Terminal, CMD. `cd sm64-vita`
4. Place a Super Mario 64 ROM called **"baserom.VERSION.z64"** into the repository's root directory for asset extraction, where **"VERSION"** can be `us`, `jp`, or `eu`
5. Run these commands: `./build_deps.sh`, `make TARGET_VITA=1 vpk`
6. The installable VPK file will be found in `sm64-vita-master/build/<VERSION>_vita`

### Notes
  
- TAS Input stops working if the app is suspended or the Vita is put to sleep.
  
## 👾 Max Payne

This **[Max Payne](https://github.com/fgsfdsfgs/max_vita)** port has been ported from **[fgsfdsfgs](https://github.com/fgsfdsfgs/)** and it uses a legally purchased APK 1.7 version of Max Payne. (This port mostly uses TheOfficialFlow ports way)

### Installation

1. Create a directory in `ux0:data/` folder, call it **"maxpayne"**
2. Extract **"assets"** folder from your APK to `ux0:data/maxpayne` folder.
3. Extract **"libMaxPayne.so"** file from your APK in `lib/armeabi-v7a` folder to `ux0:data/maxpayne` folder.
4. Extract **".obb"** file from your APK to `ux0:data/maxpayne` folder.
5. Extract **[data.zip](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/MaxPayne-data.zip)** to `ux0:data` folder.
6. Install this **[VPK file.](https://github.com/ZHassanQ/Vita-Guide/releases/download/Assets/MaxPayne_r4.vpk)** (It will create a shortcut in LiveArea) 

### Notes

The Vita port has an extra config file, located at `ux0:/data/maxpayne/config.txt` It is created when you first run the game and allows you to tweak some internal settings. For more detailed descriptions of said settings check the **[wiki article.](https://github.com/fgsfdsfgs/max_vita/wiki/Config-variables)**

- If the error says Could not find symbol, that likely means you have the wrong APK version. You need one for v1.7, others will not work.