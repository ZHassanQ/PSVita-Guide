# **CREDITS**

This MD file is fully copied from **[VitaGrafix Confiurator Repository](https://github.com/Kirezar/VitaGrafixConfigurator)** with some changes.

# ![VitaGrafix Configurator](https://i.imgur.com/hIdE4yQ.png)
A GUI Configurator for the VitaGrafix plugin

[Download Here](https://github.com/ZHassanQ/PSVita-Guide/releases/download/PRX/VitaGrafix.suprx)

## Requirements

This app requires the [instalation](https://github.com/ZHassanQ/PSVita-Guide/blob/main/Plugins.md#-3-vitagrafix) of [VitaGrafix by Electry](https://github.com/Electry/VitaGrafix)

The configurator is compatible with **VitaGrafix v5.0**+

## Usage

After opening the app, if you don't have a **"config.txt"** file on `ux0:/data/VitaGrafix` or it wasn't updated to the latest version, the app will do that for you.

You'll be greeted by a VitaGrafix Settings screen, which contains the override settings for Enabled and OSD

![Main Menu](https://i.imgur.com/B9W4YxB.png)

### Controls

* **Up and Down on the DPAD:** Move the selection up or down

* **Cross:**
  * If the selected button is the **"Enable"** or **"OSD"** then it will toggle them On or Off (If marked by an X then they are On, if empty then they are Off)
  * If the selected button is the **"Internal Resolution"** button, the app will open the Keyboard where you can type the intended Internal Resolution. This resolution can be anything with a width between 0 (exclusive) and 960 (inclusive), and a height between 0 (exclusive) and 544 (inclusive) and has to follow the format: WxH. The Internal Resolution mod can also be set to "OFF" by inputing that into the text field. Some games also support multiple resolutions in this field, separated by a ",".
  * If the selected button is the Save Config button, it will save the entire config.

* **Left and Right on the DPAD:**
  * If the selection is on the game list, it will scroll through the games
  * If the selection is either on Framebuffer or FPS, it will scroll through the available modes for those options
  
 * **Triangle:** If the selection is on any of the fields that have a (Default:) text in front of them, it will set those fields to the default value. The default value is the VitaGrafix plugin default and not the game default.
 
 * **L and R:** Moves trough the list of games (same as Left and Right but without the need of selecting the game list)
 
 ![Game screen](https://i.imgur.com/Xxgx0Ws.png)
 
 ### Saving
 
 After you are done setting the options to your liking, just press the Save Config button
 
 ## Cautions
 
 Not every option available might be compatible with each game, please refer to the [compatibility table on the VitaGrafix patchlist github page](https://github.com/ZHassanQ/PSVita-Guide/blob/main/VitaGrafix-Patches.md) - [Original](https://github.com/Electry/VitaGrafixPatchlist#supported-games)
