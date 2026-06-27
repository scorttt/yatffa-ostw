# **Yet Another Tryhard FFA**

**YATFFA** is a Tryhard FFA Workshop mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop). 

**[workshop.codes/BKRXY](https://workshop.codes/BKRXY)**

Flexibility is the core philosophy, it aims to offer extensive customization options for both the lobby host and individual players.

Inspired by the Tryhard FFA lobbies hosted by Immanust in 2018/2019, YATFFA aims to recreate that experience with modern feature comforts.

---

## Features

### Extensive Workshop Settings for Lobby hosts
- Customize a slew of options for your lobby via Workshop Settings

### In-Game Cursor Menu
- Access and modify settings at anytime mid-game:
    - HUD visibility
    - Heal reward options
    - Random hero toggle
    - Language select

### Favorites
- Pin a frequently used option without opening the full menu. Press reload on a menu item, then double-tap interact to toggle without opening the full menu
    
### Heal Rewards
- Choose between no heal rewards, kill-based healing, or healing pickups
    
### Healing Interrupted by Damage
- Taking damage pauses any ongoing healing effects
    
### Instant Respawn with interact
- Respawn instantly by pressing interact while dead
    
### Custom localization
- Choice between English, Japanese, and Korean, with future languages planned (maybe)
    
### Kill Streaks
- Live insight on who's doing well in your lobby
    
### Dynamic Stats
- Dynamic, hero specific statistics
    
### Railings Destroyed on Round Start
- Games start with railings destroyed, preventing shots from being blocked

### AFK Detection
- Automatically tags inactive players, eventually kicking them if they remain AFK for too long

---

## Known issues
- Some heroes may have incorrect generic accuracy statistics, this is an Overwatch bug
- Opening the menu will cause framerate drops due to how the in-world text updates. This is a Workshop limitation and cant be changed without sacrificing the flexibility of in-world texts that the menu utilizes

---

## Import Codes

| Region | Code |
|--------|------|
| NA/EU | `BKRXY` |
| JP | `5RKYY` |

---

## Compiling

### Prerequisites
- [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/wiki/Getting-Started) installed and set-up correctly
- [`macros-ostw`](https://github.com/scorttt/macros-ostw) repository cloned adjacent to YATFFA's parent directory

Expected folder structure:

```
scripts/
├── macros-ostw/
│   ├── main.del
│   └── ...
└── yatffa-ostw/
    ├── main.del
    └── ...
```

With YATFFA's `main.del` open and focused in VSCode, press `Ctrl+Alt+C` to copy the compiled workshop code into your clipboard that can then be pasted into Overwatch.
Please note that Flatpak/Snap builds of VSCode do not share the clipboard with other applications, use VSCode's output window instead; otherwise you'll have to figure something else out for a workaround.

### Linux

If you're using a VSCode fork such as VSCodium or Code OSS, you'll have to install the extension manually since OSTW is not listed on the Open VSX registry, you can download the VSIX from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Deltin.overwatch-script-to-workshop) directly and install it manually.

You may also need to set execute permissions on the language server binary:

```bash
# adjust the path and version number to match your install
chmod 755 ~/.config/Code\ -\ OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v3.2.3-linux-x64/Deltinteger
```

In the OSTW extension settings, set the Deltinteger path with quotes:

```
"/home/user/.config/Code - OSS/User/globalStorage/deltin.overwatch-script-to-workshop/Server/v3.2.3-linux-x64/Deltinteger"
```
