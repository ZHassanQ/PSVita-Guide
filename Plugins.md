# Plugins

This is the **"Plugins.md"** file contains every plugin i suggest and how to install them and use them. If you want them all easily go to this **[section](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#x-all-in-one)** (It doesn't contain the PSP plugins) if you want the PSP (Adrenaline) plugins go to this **[section](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#xi-psp-plugins-second-stick--enhancements)**

🧭 Table of Contents
- 🗝 Input
  - **[ReVita](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-1-revita)**
  - **[DS34](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-2-ds34vita--ds34motion)**
- 🔆 Enhances
  - **[VitaGrafix](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-3-vitagrafix)**
  - **[NoPowerLimitsVita](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-7-nopowerlimitsvita)**
- 🎞️ Media
  - **[TrophyShot](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#%EF%B8%8F-8-trophyshot)**
  - **[PNGShot](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#%EF%B8%8F-9-pngshot)**
- 🎨 Appearance
  - **[Quick Menu Plus](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-6-quick-menu-plus)**
- 🍂 Miscellaneous
  - **[BetterTrackPlug](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-4-bettertrackplug)**
  - **[StayBright](https://github.com/ZHassanQ/Vita-CFW-Guide/blob/main/Plugins.md#-5-staybright)**

## 🗝 1. ReVita

**[ReVita](https://github.com/MERLev/reVita)** a plugin for PS Vita / PS TV, which allows you to remap inputs and trigger different actions. To use it press the Select + Square.


### Installation
 
1. Copy **[ioplus.skprx]()** to `ur0:tai` folder, add **"ioplus.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[reVita.skprx]()** to `ur0:tai` folder, add **"reVita.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section. 
- Should be installed before ds34vita/ds4touch in tai config.
- Optional, to get Gyro support: Copy **[reVitaMotion.suprx]()** to `ur0:tai` folder, add **"reVitaMotion.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed (ur0:)

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

1. Copy **[ds34vita.skprx]()** to `ur0:tai` folder, add **"ds34vita.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[ds34motion.skprx]()** to `ux0:tai` folder, add **"ds34motion.skprx"** into your `ux0:tai/"config.txt"` file under **"• KERNEL"** section.
3. Copy **[ds34motion.suprx]()** to `ux0:tai` folder, add **"ds34motion.suprx"** into your `ux0:tai/"config.txt"` file under **"• TITLEID00"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/ds34vita.skprx

```

### Installed (ux:)

```

• KERNEL

ux0:tai/ds34motion.skprx


• TITLEID00
# Replace it with your game's TITLEID. Or "ALL" to affect all titles.

ux0:tai/ds34motion.suprx

```

### Notes (DS34Motion)

- If a DualShock 3 controller is used, it must not be directly plugged with USB on the PS TV otherwise, signal will be sent through USB instead of BlueTooth (and it won't be catched): use an external charger for the controller.
- It doesn't work well on classic PS Vita with "ds3vita": for an unknown reason, motion control samples seems to be too much spaced over time.
- Computed orientation is wrong when the controller is turned upside down (it could happen in a game when you try to look too verticaly high).
- Currently, gyroscope data is not exploited during orientation compute (due to drift problems I had when I tried), feel free to give help if you have some maths/IMU skills!
- Some games could be perceived like they have inverted horizontal controls (specially during FPS and TPS viewpoints) but it is a wrong impression (on a real PS Vita, tilting the device on the left also makes the view goes to the right and vice versa).

## 🔆 3. VitaGrafix

**[VitaGrafix](https://github.com/Electry/VitaGrafix)** a plugin that allows you to change resolution and FPS cap of PS Vita games. (To get better visuals, higher FPS or longer battery life) Read **["VitaGrafix.md"]()** file to see how to use this plugin.

### Installation

1. Copy **[ioplus.skprx]()** to `ux0:tai` folder, add **"ioplus.skprx"** into your `ux0:tai/"config.txt"` file under **"• KERNEL"** section.
2. Copy **[VitaGrafix.suprx]()** to `ux0:tai` folder, add **"VitaGrafix.suprx"** into your `ux0:tai/"config.txt"` file under **"• ALL"** section.

### Installed (ux0:)

```

• KERNEL

ux0:tai/ioplus.skprx


• ALL

ux0:tai/VitaGrafix.suprx

```

## 🔆 4. NoPowerLimitsVita

**[NoPowerLimits](https://github.com/Electry/NoPowerLimitsVita)** a plugin that removes some restrictions like: 77% Brightness limit, Disabled WLAN (network features), & Disabled camera.

### Installation

1. Copy **[NoPowerLimits.skprx]()** to `ur0:tai` folder, add **"NoPowerLimits.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/NoPowerLimits.skprx

```

## 🎞️ 5. TrophyShot

**[TrophyShot](https://github.com/FMudanyali/TrophyShot)** plugin that takes a screenshot when you get a trophy.

### Installation

1. Copy **[TrophyShot.suprx]()** to `ur0:tai` folder, add **"TrophyShot.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed (ur0:)

```

• MAIN

ur0:tai/TrophyShot.suprx

```

## 🎞️ 6. PNGShot

**[PngShot](https://github.com/xyzz/pngshot)**  plugin to make screenshots great again. Press PS button + Start to take a screenshot. You can access screenshots with the Photos app, or from `ux0:picture/SCREENSHOT` folder.

### Installation

1. Copy **[pngshot.suprx]()** to `ur0:tai` folder, add **"pngshot.suprx"** into your `ur0:tai/"config.txt"` file under **"• MAIN"** section.

### Installed (ur0:)

```

• MAIN

ur0:tai/pngshot.suprx

```

## 🎨 7. Quick Menu Plus

**[Quick Menu Plus](https://forum.devchroma.nl/index.php/topic,78.html)** merges Quick Power, Quick Volume, and Rapidmenu, as well as adding new features and style enhancements for the Quick Menu.

### Installation

1. Copy **[quickmenuplus.suprx]()** to `ur0:tai` folder, add **"quickmenuplus.suprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/quickmenuplus.suprx

```

### Notes

- Download and extract this file in the directory `ur0:/data/quickmenuplus` to configure Quick Menu Plus.
- **"standbyisrestart.txt"** sets the standby button to function as a restart button. Put in the file **"1"** to enable, or **"0"** to disable. If the file does not exist, the default is enabled on the Vita, and disabled on the PSTV. When this setting is disabled, hold the **"Power Off ・ Restart"** button to restart, and press to power off.
- **"bgstyle.txt"** sets the background style. Put in the file **"0"** for original, **"1"** for translucent, and **"2"** for black. If the file does not exist, the default is translucent. Black can reduce power consumption for OLED screens. The gradient effect is removed in all styles.

## 🍂 8. BetterTrackPlug

**[BetterTrackPlug](https://github.com/fmudanyali/BetterTrackPlug)** a plugin that keeps track of how long you played your games. (To display your playtime use **[BetterTrackPlug App]()**)

### Installation 

1. Copy **[BetterTrackPlug.skprx]()** to `ur0:tai` folder, add **"BetterTrackPlug.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/BetterTrackPlug.skprx

```

### Notes (App)

I would advise you to set up your bubbles in a way that their title ID's will be the same as the corresponding PSP game's title ID instead of the default PSPEMUXXX, this way, they will use the same file that stores the playtime and you won't see the game twice on the list if you launch it both from bubble or directly from adrenaline.

## 🍂 9. StayBright

**[StayBright](https://www.psx-place.com/resources/staybright.1032)** a plugin disables screen auto-dimming but retain auto-suspend. (Useful if you want to watch videos)

### Installation 

1. Copy **[staybright.skprx]()** to `ur0:tai` folder, add **"staybright.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/staybright.skprx

```

## X. All in One

If you want all the suggested plugins you can easily download this **[file.]()** And extract it in the root of your SD Card. Also you will need to copy this code block:

```

• KERNEL

ur0:tai/ioplus.skprx
ur0:tai/reVita.skprx
ur0:tai/ds34vita.skprx
ur0:tai/BetterTrackPlug.skprx
ur0:tai/staybright.skprx
ur0:tai/quickmenuplus.suprx
ur0:tai/NoPowerLimits.skprx

• MAIN

ur0:tai/reVitaMotion.suprx
ur0:tai/TrophyShot.suprx
ur0:tai/pngshot.suprx

```

And paste it to your `ur0:tai/"config.txt` file. And copy this code block:

```

• KERNEL

ux0:tai/ioplus.skprx
ux0:tai/ds34motion.skprx

• ALL

ux0:tai/VitaGrafix.suprx
ux0:tai/ds34motion.suprx

```

And paste it to your `ux0:tai/"config.txt"` file.

## XI. PSP Plugins (Second Stick & Enhancements)

- **[GTANativeRes](https://github.com/TheOfficialFloW/GTANativeRes)** Internal resolution patch for PSP GTA series.
- **[RemasteredControls](https://github.com/TheOfficialFloW/RemasteredControls)** A collection of dual analog patches for PSP games on Adrenaline.
- **[PSP-Camera_Patch_Lite](https://github.com/Freakler/psp-camera_patch_lite)** More collection of dual analog patches for PSP games on Adrenaline.
- **[GePatch](https://github.com/TheOfficialFloW/GePatch)** Enables native resolution in a few PSP games. (If a **[game crashed](https://docs.google.com/spreadsheets/d/1aZlmKwELcdpCb9ezI5iRfgcX9hoGxgL4tNC-673aKqk/edit#gid=0)** launch it while holding the R button to skip GePatch)

### Installation

This installation process applies to every PSP plugin. The difference is the plugin name.

1. Copy **[gta_native.prx]()** to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/gta_native.prx 1"** into your `ux0:pspemu/seplugins/"game.txt"`
2. Download and extract this **[remastered file]()** in the root of your SD Card and copy this code block into your: `ux0:pspemu/seplugins/"game.txt`
3. Copy **[camera_patch_lite.ini]()** & [camera_patch_lite.prx]() to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/camera_patch_lite.prx 1"** into your `ux0:pspemu/seplugins/"game.txt"`
4. Copy **[ge_patch.prx]()** to `ux0:pspemu/seplugins/` folder, add **"ms0:seplugins/ge_patch 1"** into your `ux0:pspemu/seplugins/"game.txt"`

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
