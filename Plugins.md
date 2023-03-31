# Plugins


## 1. ReVita

**[ReVita](https://github.com/MERLev/reVita)** a plugin for PS Vita / PS TV, which allows you to remap inputs and trigger different actions.


### Installation
 
1. Copy **[ioplus.skprx]()** to `ur0:/tai` folder, add **"ioplus.skprx"** into your `ur0:/config.txt` file under "• KERNEL" section.
2. Copy **[reVita.skprx]()** to `ur0:/tai` folder, add **"reVita.skprx"** into your `ur0:/config.txt` file under "• KERNEL" section. 
- Should be installed before ds34vita/ds4touch in tai config.
- Optional, to get Gyro support: Copy **[reVitaMotion.suprx]()** to `ur0:/tai` folder, add **"reVitaMotion.suprx"** into your `ur0:/"config.txt"` file under "• MAIN" section.

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

## 2. DS34Vita & DS34Motion

**[DS34Vita](https://github.com/MERLev/ds34vita)** adds DualShock 3, 4, & Dualsense support to your PSVita. And **[DS34Motion](https://github.com/MERLev/DS34Motion) adds motion support to your DualShock 3, 4 controllers to your PSVita.

### Installation

1. Copy **[ds34vita.skprx]()** to `ur0:/tai` folder, add **"ds34vita.skprx"** into your `ur0:/config.txt` file under "• KERNEL" section.
2. Copy **[ds34motion.skprx]()** to `ur0:/tai` folder, add **"ds34motion.skprx"** into your `ur0:/config.txt` file under "• KERNEL" section.
3. Copy **[ds34motion.suprx]()** to `ur0:/tai` folder, add **"ds34motion.suprx"** into your `ur0:/config.txt` file under "• TITLEID00" section.

### Installed

```
• KERNEL

ur0:tai/ds34vita.skprx
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

## 3.


## 4.
