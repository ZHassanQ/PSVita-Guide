# Plugins

This is the **"Plugins.md"** file contains every plugin i suggest and how to install them and use them. Note that Vita plugins are always in `ur0:tai` folder and PSP plugins are always in `ux0:pspemu/seplugins/` folder. If you want them all easily go to this **[section](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#xv-all-in-one)** (It doesn't contain the PSP plugins) if you want the PSP (Adrenaline) plugins go to this **[section.](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#xvi-psp-plugins-second-stick--enhancements)**

🧭 Table of Contents
- 🗝 Input
  - **[ReVita](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-1-revita)**
  - **[DS34](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-2-ds34vita--ds34motion)**
- 🔆 Enhances
  - **[VitaGrafix](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-3-vitagrafix)**
  - **[NoPowerLimitsVita](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-4-nopowerlimitsvita)**
- 🚀 Overclocking
  - **[CapUnlocker](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-5-CapUnlocker)**
  - **[PSVshellPlus](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-6-psvshellplus)**
- 🎞️ Media
  - **[TrophyShot](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#%EF%B8%8F-7-trophyshot)**
  - **[PNGShot](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#%EF%B8%8F-8-pngshot)**
- 🎨 Appearance
  - **[Quick Menu Plus](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-9-quick-menu-plus)**
  - **[Vita Shellbat](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-x-vita-shellbat)**
- 🍂 Miscellaneous
  - **[BetterTrackPlug](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-xi-bettertrackplug)**
  - **[Download Enabler](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-xii-vita-shellbat)**
  - **[StayBright](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-xiii-staybright)**
  - **[VitaBright](https://github.com/ZHassanQ/Vita-Guide/blob/main/Plugins.md#-xiv-vita-shellbat)**

## 🗝 1. ReVita

**[ReVita](https://github.com/MERLev/reVita)** a plugin for PS Vita / PS TV, which allows you to remap inputs and trigger different actions. To use it press the Select + Square.


### Installation
 
1. Copy **[ioplus.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ioplus.skprx)** to `ur0:tai` folder, add **"ioplus.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[reVita.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/reVita.skprx)** to `ur0:tai` folder, add **"reVita.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section. 
- Should be installed before ds34vita/ds4touch in tai config.
- Optional, to get Gyro support: Copy **[reVitaMotion.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/reVitaMotion.suprx)** to `ur0:tai` folder, add **"reVitaMotion.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed

```

• KERNEL

ur0:tai/ioplus.skprx
ur0:tai/reVita.skprx


• MAIN

ur0:tai/reVitaMotion.suprx

```

### Notes

- Adrenaline - to get UI working, you need to change **"Adrenaline Settings"** -> **"Graphics Filtering"** to anything else except original.
- In some of hombrews and PSP/PS1 games GUI won't work - use Shared profile method for them: Save it as Shared profile **"Profile"** --> **"Profile management"** --> **"Save as Shared"**

## 🗝 2. DS34Vita & DS34Motion

**[DS34Vita](https://github.com/MERLev/ds34vita)** adds DualShock 3, 4, & Dualsense support to your PSVita. And **[DS34Motion](https://github.com/MERLev/DS34Motion)** adds motion support to your DualShock 3, 4 controllers to your PSVita.

### Installation

1. Copy **[ds34vita.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ds34vita.skprx)** to `ur0:tai` folder, add **"ds34vita.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[ds34motion.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ds34motion.skprx)** to `ur0:tai` folder, add **"ds34motion.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
3. Copy **[ds34motion.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ds34motion.suprx)** to `ur0:tai` folder, add **"ds34motion.suprx"** into your `ur0:tai/"config.txt"` file under **"• TITLEID00"** section.

### Installed

```

• KERNEL

ur0:tai/ds34vita.skprx
• KERNEL

ur0:tai/ds34motion.skprx


• TITLEID00
# Replace it with your game's TITLEID. Or "ALL" to affect all titles.

ur0:tai/ds34motion.suprx

```

### Notes (DS34Motion)

- If a DualShock 3 controller is used, it must not be directly plugged with USB on the PS TV otherwise, signal will be sent through USB instead of BlueTooth (and it won't be catched): use an external charger for the controller.
- It doesn't work well on classic PS Vita with "ds3vita": for an unknown reason, motion control samples seems to be too much spaced over time.
- Computed orientation is wrong when the controller is turned upside down (it could happen in a game when you try to look too verticaly high).
- Currently, gyroscope data is not exploited during orientation compute (due to drift problems I had when I tried), feel free to give help if you have some maths/IMU skills!
- Some games could be perceived like they have inverted horizontal controls (specially during FPS and TPS viewpoints) but it is a wrong impression (on a real PS Vita, tilting the device on the left also makes the view goes to the right and vice versa).

## 🔆 3. VitaGrafix

**[VitaGrafix](https://github.com/Electry/VitaGrafix)** a plugin that allows you to change resolution and FPS cap of PS Vita games. (To get better visuals, higher FPS or longer battery life) Read **["VitaGrafix.md"](https://github.com/ZHassanQ/Vita-Guide/blob/main/VitaGrafix.md)** file to see how to use this plugin.

### Installation

0. Download this **[file](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/VitaGrafix-Patches-List.zip)** and extract it in `ux0:data/VitaGrafix` folder.
1. Copy **[ioplus.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ioplus.skprx)** to `ur0:tai` folder, add **"ioplus.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[VitaGrafix.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/VitaGrafix.suprx)** to `ur0:tai` folder, add **"VitaGrafix.suprx"** into your `ur0:tai/"config.txt"` file under **"• ALL"** section.

### Installed

```

• KERNEL

ur0:tai/ioplus.skprx


• ALL

ur0:tai/VitaGrafix.suprx

```

## 🔆 4. NoPowerLimitsVita

**[NoPowerLimits](https://github.com/Electry/NoPowerLimitsVita)** a plugin that removes some restrictions like: 77% Brightness limit, Disabled WLAN (network features), & Disabled camera.

### Installation

1. Copy **[NoPowerLimits.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/NoPowerLimits.skprx)** to `ur0:tai` folder, add **"NoPowerLimits.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/NoPowerLimits.skprx

```

## 🚀 5. CapUnlocker

**[CapUnlocker](https://github.com/GrapheneCt/CapUnlocker)** allows to use system reserved 4th CPU core and other capabilities. (Mainly used for heavy games and/or ports)

### Installation 

1. Copy **[CapUnlocker.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/CapUnlocker.skprx)** to `ur0:tai` folder, add **"CapUnlocker.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/CapUnlocker.skprx

```
 
## 🚀 6. PSVshellPlus

**[PSVshell](https://github.com/Electry/PSVshell)** overclock plugin with FPS counter and CPU usage (Mainly used for heavy games and/or ports)

### Installation 

1. Copy **[PSVshell.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/PSVshell.skprx)** to `ur0:tai` folder, add **"PSVshell.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/PSVshell.skprx

```

### Notes

- Press SELECT + UP or SELECT + DOWN to toggle between 3 GUI modes

- When in 'FULL' mode:

  - Use UP/DOWN to move in the menu
  - Press X to toggle frequency mode for currently selected > device <:
    - Default freq. (WHITE) - the plugin will not interfere, but rather use the default freq. for current game
    - Manual freq. (BLUE) - the plugin will use your specified freq.
      - press LEFT/RIGHT to immediately change the frequency
  - Press X when > save profile < is selected to save/delete profiles
    - All Manual freq. (BLUE) will be loaded and applied next time you start/resume the game
    - All Default freq. (WHITE) will be kept to default (set to whatever freq. the game asks for)
  - Press and hold LEFT TRIGGER and > save profile < will change to > save global <
    - Press X when > save global < is selected and the options will be saved to global (default) profile
    - Global profile will be used as default profile when game-specific profile doesn't exist
 
## 🎞️ 7. TrophyShot

**[TrophyShot](https://github.com/FMudanyali/TrophyShot)** plugin that takes a screenshot when you get a trophy.

### Installation

1. Copy **[TrophyShot.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/TrophyShot.suprx)** to `ur0:tai` folder, add **"TrophyShot.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed

```

• MAIN

ur0:tai/TrophyShot.suprx

```

## 🎞️ 8. PNGShot

**[PngShot](https://github.com/xyzz/pngshot)**  plugin to make screenshots great again. Press PS button + Start to take a screenshot. You can access screenshots with the Photos app, or from `ur0:picture/SCREENSHOT` folder.

### Installation

1. Copy **[pngshot.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/pngshot.suprx)** to `ur0:tai` folder, add **"pngshot.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed

```

• MAIN

ur0:tai/pngshot.suprx

```

## 🎨 9. Quick Menu Plus

**[Quick Menu Plus](https://forum.devchroma.nl/index.php/topic,78.html)** merges Quick Power, Quick Volume, and Rapidmenu, as well as adding new features and style enhancements for the Quick Menu.

### Installation

1. Copy **[quickmenuplus.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/quickmenuplus.suprx)** to `ur0:tai` folder, add **"quickmenuplus.suprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/quickmenuplus.suprx

```

### Notes

- Download and extract this file in the directory `ur0:/data/quickmenuplus` to configure Quick Menu Plus.
- **"standbyisrestart.txt"** sets the standby button to function as a restart button. Put in the file **"1"** to enable, or **"0"** to disable. If the file does not exist, the default is enabled on the Vita, and disabled on the PSTV. When this setting is disabled, hold the **"Power Off ・ Restart"** button to restart, and press to power off.
- **"bgstyle.txt"** sets the background style. Put in the file **"0"** for original, **"1"** for translucent, and **"2"** for black. If the file does not exist, the default is translucent. Black can reduce power consumption for OLED screens. The gradient effect is removed in all styles.

## 🎨 X. Vita Shellbat

**[Vita Shellbat](https://github.com/nowrep/vita-shellbat)** a plugin that shows battery percent in statusbar.

### Installation

1. Copy **[shellbat.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/shellbat.suprx)** to `ur0:tai` folder, add **"shellbat.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed

```

• MAIN

ur0:tai/shellbat.suprx

```

## 🍂 XI. BetterTrackPlug

**[BetterTrackPlug](https://github.com/fmudanyali/BetterTrackPlug)** a plugin that keeps track of how long you played your games. (To display your playtime use **[BetterTrackPlug App](https://github.com/ZHassanQ/Vita-Guide/releases/download/VPK/BetterTrackPlug.vpk)**)

### Installation 

1. Copy **[BetterTrackPlug.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/BetterTrackPlug.skprx)** to `ur0:tai` folder, add **"BetterTrackPlug.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/BetterTrackPlug.skprx

```

### Notes (App)

I would advise you to set up your bubbles in a way that their title ID's will be the same as the corresponding PSP game's title ID instead of the default PSPEMUXXX, this way, they will use the same file that stores the playtime and you won't see the game twice on the list if you launch it both from bubble or directly from adrenaline.

## 🍂 XII. Download Enabler

**[Download Enabler](https://github.com/TheOfficialFloW/VitaTweaks#2-download-enabler) allows you to download any content from the webbrowser to `ux0:download` folder.

### Installation

1. Copy **[download_enabler.suprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/download_enabler.suprx)** to `ur0:tai` folder, add **"download_enabler.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed

```

• MAIN

ur0:tai/download_enabler.suprx

```

## 🍂 XIII. StayBright

**[StayBright](https://www.psx-place.com/resources/staybright.1032)** a plugin disables screen auto-dimming but retain auto-suspend. (Useful if you want to watch videos)

### Installation 

1. Copy **[staybright.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/staybright.skprx)** to `ur0:tai` folder, add **"staybright.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• KERNEL

ur0:tai/staybright.skprx

```

## 🍂 XIV. VitaBright

**[VitaBright](https://github.com/devnoname120/vitabright)** plugin enables you to alter the luminosity levels of your PS Vita. It thus allows you to decrease the brightness level below the minimum, and increase it above the maximum.

### Installation

0. Download this **[file](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/VitaBright_Lut.zip)** and extract it in `ur0:tai` folder.
1. Copy **[vitabright.skprx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/vitabright.skprx)** to `ur0:tai` folder, add **"vitabright.suprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed

```

• MAIN

ur0:tai/vitabright.skprx

```

### Notes

- Once vitabright is installed and your Vita is restarted, it will automatically work. Just open the brightness settings and move the slider.
- You can customize the gamma table that vitabright uses for OLED screens (PS Vita 1000): open the file vitabright_lut.txt and modify it according to your needs. Note: for now, you cannot tweak the luminosity levels of LCD screens (PS Vita 2000) without recompiling the plugin (for advanced users).
- Note that while there is also a file named vitabright_lut_orig.txt, it's not used by vitabright and it's only here for informational purposes.
- If you want to edit the OLED gamma table then use this **[app.]((https://github.com/ZHassanQ/Vita-Guide/releases/download/VPK/vitabright-lut-editior-1.1.vpk)** ([OLED Gamma Table Explanation](https://github.com/devnoname120/vitabright/wiki/What-is-the-format-of-the-OLED-gamma-table%3F)**)

## XV. All in One

If you want all the suggested plugins you can easily download these **[AIO-Plugins](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/AIO-Plugins.zip)**, **[VitaBright-Lut](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/VitaBright_Lut.zip)**, **[VitaGrafix-Patches-list](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/VitaGrafix-Patches-List.zip)** files. And extract them in:

- AIO-Plugins in `ur0:tai` folder.
- VitaBright-Lut in `ur0:tai` folder.
- VitaGrafix-Patches-List in `ux0:data/VitaGrafix` folder.

After that copy the code block down and paste it in `ur0:tai/"config.txt"` file.

```

• KERNEL

ur0:tai/ioplus.skprx
ur0:tai/reVita.skprx
ur0:tai/ds34vita.skprx
ur0:tai/ds34motion.skprx
ur0:tai/BetterTrackPlug.skprx
ur0:tai/staybright.skprx
ur0:tai/quickmenuplus.suprx
ur0:tai/NoPowerLimits.skprx
ur0:tai/CapUnlocker.skprx
ur0:tai/PSVshell.skprx


• MAIN

ur0:tai/reVitaMotion.suprx
ur0:tai/TrophyShot.suprx
ur0:tai/pngshot.suprx
ur0:tai/shellbat.suprx
ur0:tai/vitabright.skprx
ur0:tai/download_enabler.suprx


• ALL

ur0:tai/VitaGrafix.suprx
ur0:tai/ds34motion.suprx

```

## XVI. PSP Plugins (Second Stick & Enhancements)

- **[GTANativeRes](https://github.com/TheOfficialFloW/GTANativeRes)** Internal resolution patch for PSP GTA series.
- **[RemasteredControls](https://github.com/TheOfficialFloW/RemasteredControls)** A collection of dual analog patches for PSP games on Adrenaline.
- **[PSP-Camera_Patch_Lite](https://github.com/Freakler/psp-camera_patch_lite)** More collection of dual analog patches for PSP games on Adrenaline.
- **[GePatch](https://github.com/TheOfficialFloW/GePatch)** Enables native resolution in a few PSP games. (If a **[game crashed](https://docs.google.com/spreadsheets/d/1aZlmKwELcdpCb9ezI5iRfgcX9hoGxgL4tNC-673aKqk/edit#gid=0)** launch it while holding the R button to skip GePatch)

### Installation

This installation process applies to every PSP plugin. The difference is the plugin name.

1. Copy **[gta_native.prx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/gta_native.prx)** to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/gta_native.prx 1"** into your `ux0:pspemu/seplugins/"game.txt"`
2. Download and extract this **[remastered file](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/Remastered-PSP-Plugins.zip)** in the root of your SD Card and copy the **"remastered"** code block into your: `ux0:pspemu/seplugins/"game.txt"`
3. Copy **[camera_patch_lite.ini](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/camera_patch_lite.ini)** & **[camera_patch_lite.prx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/camera_patch_lite.prx)** to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/camera_patch_lite.prx 1"** into your `ux0:pspemu/seplugins/"game.txt"`
4. Copy **[ge_patch.prx](https://github.com/ZHassanQ/Vita-Guide/releases/download/PRX/ge_patch.prx)** to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/ge_patch 1"** into your `ux0:pspemu/seplugins/"game.txt"`

### Installed (ux0:pspemu/)

```

# To disable a plugin set the plugin line to false 0.

ms0:seplugins/gta_native.prx 1
ms0:seplugins/gta_remastered_v2.prx 1
ms0:seplugins/resistance_remastered.prx 1
ms0:seplugins/splintercell_remastered.prx 1
ms0:seplugins/tombraider_remastered.prx 1
ms0:seplugins/pop_remastered.prx 1
ms0:seplugins/khbbs_remastered.prx 1
ms0:seplugins/mgs_remastered.prx 1
ms0:seplugins/warriors_remastered.prx 1
ms0:seplugins/tonyhawk_remastered.prx 1
ms0:seplugins/camera_patch_lite.prx 1
ms0:seplugins/ge_patch 1

```
