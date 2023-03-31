# Plugins


## 1. ReVita

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

## 2. DS34Vita & DS34Motion

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

## 3. VitaGrafix

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

## 4. BetterTrackPlug

**[BetterTrackPlug](https://github.com/fmudanyali/BetterTrackPlug)** A plugin that keeps track of how long you played your games. (To display your playtime use **[BetterTrackPlug App]()**)

### Installation 

1. Copy **[BetterTrackPlug.skprx]()** to `ur0:tai` folder, add **"BetterTrackPlug.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/BetterTrackPlug.skprx

```

### Notes (App)

I would advise you to set up your bubbles in a way that their title ID's will be the same as the corresponding PSP game's title ID instead of the default PSPEMUXXX, this way, they will use the same file that stores the playtime and you won't see the game twice on the list if you launch it both from bubble or directly from adrenaline.

## 4. StayBright

**[StayBright](https://www.psx-place.com/resources/staybright.1032)** plugin disables screen auto-dimming but retain auto-suspend. (Useful if you want to watch videos)

### Installation 

1. Copy **[staybright.skprx]()** to `ur0:tai` folder, add **"staybright.skprx"** into your `ur0:tai/"config.txt"` file under **"• KERNEL"** section.

### Installed (ur0:)

```

• KERNEL

ur0:tai/staybright.skprx

```

## 6. Quick Menu Plus

**[Quick Menu Plus]($**
