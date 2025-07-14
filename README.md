# **Yet Another Tryhard FFA**
[workshop.codes post](https://workshop.codes/BKRXY)

**YATFFA** is a Tryhard FFA Workshop mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop). Flexibility is the main philosophy, it offers extensive customization options for both the lobby host and individual players.
Inspired by the Tryhard FFA lobbies hosted by Immanust in 2018/2019, YATFFA aims to recreate that experience with modern feature comforts.
# Features

- ### Extensive Workshop Settings for Lobby hosts
    Customize a slew of options for your lobby via Workshop Settings
- ### In-Game Animated Cursor Menu
    Access and modify settings anytime during gameplay:
    - HUD visibility options
    - Heal reward options
    - Random hero toggle
    - Language select
- ### Favorites
    Quickly toggle a frequently used option without opening the full menu. Press reload on a selected menu item and double tap interact to toggle
- ### Multiple Heal Reward Options
    Choose from no heal rewards, heal on kill, or healing pickups for your lobby
- ### Healing Interrupted by Damage
    Taking damage pauses any ongoing healing effects
- ### Instant Respawn with interact
    Respawn instantly by pressing interact while dead
- ### Custom localization
    Choice between English, Japanese, and Korean
- ### Kill Streaks
    Quick insight on who's doing well in your lobby
- ### Dynamic Stats
    Dynamic, hero specific statistics
- ### Railings Destroyed on Round Start
    Games start with railings destroyed, preventing shots from being interrupted by railings
- ### AFK
    Automatically tags inactive players, eventually kicking them if they remain AFK for too long

# Known issues
- Some heroes may have incorrect generic accuracy statistics, this is an Overwatch bug
- Opening the menu will cause framerate drops due to how the in-world text updates. This is a Workshop limitation and cant be changed without sacrificing the flexibility of in-world texts that the menu utilizes

# Import Codes
- `BKRXY` (NA/EU)
- `5RKYY` (JP)

# Compiling
#### Prerequisites
- [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/wiki/Getting-Started) must be set up
- My [`macros`](https://github.com/scorttt/macros-ostw) repository must be placed in a folder named `macros-ostw` next to YATFFA's parent directory

The folder structure should be as follows:
```
scripts folder
  ├ macros-ostw
  │   ├ main.del
  │   └ other macro files
  └ yatffa-ostw
      ├ main.del
      └ other yatffa files
```
With YATFFA's `main.del` focused in VSCode, press `Ctrl + Alt + C` to copy the compiled workshop code into your clipboard that can then be pasted into Overwatch, the VSCode output window is not needed, unless you are using a Flatpak/Snap version of VSCode as Flatpak/Snap versions do not share clipboards between applications.
#### Linux
If you're using a VSCode fork like VSCodium or Code OSS, you'll need to manually install the OSTW extension, as OSTW isn't available on the Open VSX registry, which is what many VSCode forks use. You can download the OSTW VSIX from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Deltin.overwatch-script-to-workshop) directly and install it manually.

You may need to adjust permissions depending on where your settings are located. Navigate to the extension directory (e.g. `~/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v3.2.3-linux-x64/`) and chmod Deltinteger accordingly:
```bash
chmod 755 Deltinteger
```

In the OSTW extension settings, wrap the Deltinteger path in quotes, for example: (change the path to your correct folder location and version number accordingly)
```
"/home/user/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v3.2.3-linux-x64/Deltinteger" 
```
