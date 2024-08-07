# **Yet Another Tryhard FFA**
[workshop.codes post](https://workshop.codes/BKRXY)

**YATFFA** is a Tryhard FFA Workshop mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop). Designed with flexibility in mind, it offers extensive customization options for both lobby hosts and players alike.

Inspired by the Tryhard FFA lobbies hosted by Immanust in 2018/2019, YATFFA aims to recreate that experience with modern feature comforts.

## Features
- **Extensive Workshop Settings for Lobby Hosts:** Customize a slew of options for your lobby
- **In-Game Animated Cursor Menu:** Access and modify settings anytime during gameplay:
    - HUD visibility options
    - Heal reward options
    - Random hero options
    - Language select
    - Vote kick
    - Changelog
- **Favorites:** Quickly toggle a frequently used option without opening the full menu
- **Multiple Heal Reward Options:** Choose from no heal rewards, heal on kill, or healing pickups for your lobby
- **Multiple Randomization Options:** Choose the randomization method used and blacklist unwanted heroes
- **Healing Interrupted by Damage:** Taking damage pauses any ongoing healing effects
- **Instant Respawn with Interact Button:** Respawn instantly by pressing interact while dead
- **Custom Language Localization:** Choice between English, Japanese, and Korean
- **Kill Streaks:** See who's doing well in your lobby
- **Dynamic, Custom Stats:** Get insights into your performance with detailed in-game statistics, including hero-specific stats and a letter grade to compare yourself to others.
- **Railings Destroyed on Round Start:** Games start with railings destroyed, stopping bullets from interrupting shots
- **AFK:** Automatically tags inactive players, eventually kicking them if they remain AFK for too long
- **Vote Kick:** Maintain lobby agency with player-driven moderation

## Known issues
- Some heroes may have inaccurate generic accuracy stats, this is an Overwatch bug
- Opening the menu can cause framerate drops due to in-world text updates. This is a Workshop limitation and cannot be changed without sacrificing the flexibility of in-world texts that the menu utilizes
- The in-game menu's positioning and button hitboxes may appear off-center on displays with aspect ratios other than 16:9 (standard monitors) or 16:10 (such as a Steam Deck)

## Import Codes
- `BKRXY` (NA/EU)
- `5RKYY` (JP)

## Compiling
#### YATFFA requires the following:
- [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/wiki/Getting-Started) must be set up
- My [`macros`](https://github.com/scorttt/macros-ostw) repository must be placed in a folder named `macros-ostw` next to YATFFA's parent directory

The folder structure should appear as follows:
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
If you are on Linux, you are likey using a VSCode fork such as VSCodium or Code OSS -- OSTW needs the VSIX to be manually installed as it's not available on the open VSX registry: https://marketplace.visualstudio.com/items?itemName=Deltin.overwatch-script-to-workshop

Deltinteger permissions needs to be set to 777 and the Deltinteger path needs to be wrapped in quotes within the extension settings if using Code OSS

(for example: `"/home/user/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v3.1.1-linux-x64/Deltinteger"`) 
