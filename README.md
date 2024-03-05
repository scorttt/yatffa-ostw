# **Yet Another Tryhard FFA**
[workshop.codes post](https://workshop.codes/BKRXY)

Workshop Tryhard FFA mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop) with the goal of being as flexible as possible for hosts and players alike

Inspired by the balance of old Tryhard FFA lobbies hosted by Immanust in 2018/2019

## Features
- In game animated cursor menu that players can access at any time to modify in game options
    - HUD visibility
    - Heal settings
        - Healing amount
        - Healing duration
    - Randomized Heroes
    - Language switching
        - English
        - Japanese
- Choice between Heal on Kill or Healing Pickups
- Taking damage interrupts healing
- Interact for Instant Respawn
- Custom EN/JP localization
- Kill streaks
- Dynamic stats
- Railings destroyed on round start
- AFK system

### Known issues
- Spectators and those viewing POTGs, kill cams, or replay viewers will see strings displayed as 0 or multiple 0's. This is a result of custom localization for every string. Since spectators and replay viewers do not have playervars, they will not be initialized and will appear incorrectly
- Some heroes will not accurately track Accuracy stats
- Opening the menu will cause a significant drop in framerate due to in-world texts updating every frame, complain to Blizzard for a better solution, as it's not something I can change while maintaining the flexibility of in-world texts

## Import Codes
- `BKRXY` (NA/EU)
- `5RKYY` (JP)
- `PBQ0A` (Fork) (Richardstone)

## Compiling
[OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/wiki/Getting-Started) must be set up and my [`macros`](https://github.com/scorttt/macros-ostw) repo must also be placed in a folder named `macros-ostw` above YATFFA's parent directory. The folder structure should appear as follows: 
```
macros-ostw
    ├ main.del
    └ other macro files

yatffa-ostw
    ├ main.del
    └ other yatffa files
```
After opening `main.del`, press `Ctrl + Alt + C` to copy the compiled workshop code into your clipboard that can then be pasted into Overwatch, VSCode output is not needed
If compiling on Linux, make sure you are not using VSCode forks such as VSCodium or Code OSS, to my knowledge only the official Microsoft version of VSCode plays nicely with OSTW.

