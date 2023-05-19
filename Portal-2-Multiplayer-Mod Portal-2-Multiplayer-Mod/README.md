
# PORTAL 2: MULTIPLAYER MOD

## Introduction

P2MM is a mod for the popular Valve game, Portal 2. It allows players to easily create lobbies with up to 32 players in both cooperative and singleplayer mods.

This mod is completely server-sided, meaning only the host needs this mod installed, the rest of the player can run Portal 2 normally.

## Features

- A maximum player cap of 32
- Nametags
- Custom Player colors
- Chat commands (!help)
- In-game Admin system
- Full cooperative campaign support
- Full singleplayer campaign support
- In-house map support for select workshop maps
- Encryption of client commands invoked through the active GameRules class
- Support for Linux, Windows 7 and above
- Togglable game options and config system exposed through VScript and a custom plugin
- Support for SAR (SourceAutoRecord) for speedrunning

## Planned Features

- Steam Deck/SteamOS 3.0 support
- More support for workshop maps
- Remote download Support

# Installation & use

**Steam guide explaining how to use the mod:**

- https://steamcommunity.com/sharedfiles/filedetails/?id=2458260280

**Downlaod latest version:**

- https://github.com/kyleraykbs/Portal2-32PlayerMod/releases/latest

**Discord Server for technical help (MAKE SURE YOU READ THE FAQ!!!), bug report or to just chat:**

- https://discord.gg/kW3nG6GKpF

# Build

*We use Python 3.10*

**Dependencies**

- pygame
- pyperclip
- requests
- steamid-converter

We also have them in a file for easy install `pip install -r requirements.txt`

**Compilation**

We use `pyinstaller` to make the executable

- Windows:

```sh
> pyinstaller "src/MainWindow.py" -F -i "src/GUI/assets/images/p2mm64.ico" --noconsole --add-data "src/GUI;GUI" --add-data "src/ModFiles;ModFiles" --add-data "src/languages;languages"
```

- Linux:

```sh
$ pyinstaller "src/MainWindow.py" -F --add-data "src/GUI:GUI" --add-data "src/ModFiles:ModFiles" --add-data "src/languages:languages"
```

*Note:*

If you want to fork the project and do your own releases you need to changes the variables at the top of `src/Scripts/Updater.py` to your own information

# Contributions

We are always happy to take whatever additional help we can get for this project. Specifically, we are in need of proficient coders in Squirrel or C++. If you think you can spare a hand, it will go a long way!

# Credits

**Developers:**

- [kyleraykbs](https://github.com/kyleraykbs)
- [Bumpy](https://github.com/BumpyAHK)
- [Nanoman2525](https://github.com/Nanoman2525)
- [vista](https://github.com/KonradCzerw)
- [Wolƒe Strider Shoσter](https://github.com/wolfestridershooter)
- [cabiste](https://github.com/cabiste69)
- [Orsell](https://github.com/OrsellGaming)

**Contributors:**

- wanderer (free bird)
- MeblIkea
- Luukex
- PieCreeper
- Areng
- /n
