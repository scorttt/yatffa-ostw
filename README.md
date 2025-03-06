# **Yet Another Tryhard FFA**
[workshop.codes post](https://workshop.codes/BKRXY)

**YATFFA** is a Tryhard FFA Workshop mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop). Designed with flexibility in mind, it offers extensive customization options for both lobby hosts and players alike.

Inspired by the Tryhard FFA lobbies hosted by Immanust in 2018/2019, YATFFA aims to recreate that experience with modern feature comforts.

## Features
- **Extensive Workshop Settings for Lobby Hosts:** Customize a slew of options for your lobby via Workshop Settings
- **In-Game Animated Cursor Menu:** Access and modify settings anytime during gameplay:
    - HUD visibility options
    - Heal reward options
    - Random hero toggle
    - Language select
- **Favorites:** Quickly toggle a frequently used option without opening the full menu. Press reload on a selected menu item and double tap interact to toggle
- **Multiple Heal Reward Options:** Choose from no heal rewards, heal on kill, or healing pickups for your lobby
- **Healing Interrupted by Damage:** Taking damage pauses any ongoing healing effects
- **Instant Respawn with Interact Button:** Respawn instantly by pressing interact while dead
- **Custom Language Localization:** Choice between English, Japanese, and Korean
- **Kill Streaks:** See who's doing well in your lobby
- **Dynamic, Custom Stats:** Get insights into your performance with detailed in-game statistics
- **Railings Destroyed on Round Start:** Games start with railings destroyed, preventing shots from being interrupted by railings
- **AFK:** Automatically tags inactive players, eventually kicking them if they remain AFK for too long

## Known issues
- Some heroes may have inaccurate generic accuracy stats, this is an Overwatch bug
- Opening the menu can cause framerate drops due to in-world text updates. This is a Workshop limitation and cannot be changed without sacrificing the flexibility of in-world texts that the menu utilizes

## Import Codes
- `BKRXY` (NA/EU)
- `5RKYY` (JP)

## Compiling
#### YATFFA requires the following:
- [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/wiki/Getting-Started) must be set up
- My [`macros`](https://github.com/scorttt/macros-ostw) repository must be placed in a folder named `macros-ostw` next to YATFFA's parent directory

The folder structure should be as follows:
```
macros-ostw
    ├ main.del
    └ other macro files

yatffa-ostw
    ├ main.del
    └ other yatffa files
```
After opening `main.del`, press `Ctrl + Alt + C` to copy the compiled workshop code into your clipboard that can then be pasted into Overwatch, VSCode output is not needed.

#### Linux
If you're using a VSCode fork like VSCodium or Code OSS, you'll need to manually install the OSTW extension, as it isn't available on the Open VSX registry. Download the OSTW VSIX from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Deltin.overwatch-script-to-workshop). 

You may need to adjust permissions based on your distro. Navigate to the extension directory (usually `~/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v#.#.#-linux-x64/`) and chmod Deltinteger:

```bash
chmod 755 Deltinteger
```

In the OSTW extension settings, wrap the Deltinteger path in quotes, for example:

```
"/home/user/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v#.#.#-linux-x64/Deltinteger"
```

