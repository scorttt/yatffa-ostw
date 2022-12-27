# **Yet Another Tryhard FFA**
[workshop.codes post](https://workshop.codes/BKRXY)

Workshop Tryhard FFA mode built on [OSTW](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop)

Inspired by the balance of old Tryhard FFA lobbies hosted by Immanust in 2018/2019

I am looking for translators for other languages! If interested, message me on discord: `scort#9899`

### Known issues
- Strings will show as 0 or multiple 0's for spectators and anyone viewing POTGs, kill cams or replay viewer; this is a side effect of having every string custom localized. Since spectators and viewers of a replay will never have playervars, they will never be initialized and will show incorrectly
- Some heroes will not accurately track Crit Accuracy
- Having the main menu open will significantly drop framerate due to the in-world texts updating every frame, complain to Blizzard instead of me for a better solution so I don't have to do this!
- Pharah bots that destroy railings will just randomly not spawn (if the lobby isn't already full), this seems to be a combination of Dummy Bot jank, workshop bugs and for some reason, host latency

## Features
- In game animated cursor menu that players can access at any time to modify in game options
    - HUD visibility
    - Heal on Kill 
    - Heal on Kill amount
    - Heal on Kill duration
    - Randomized Heroes
    - Language switching
        - English
        - Japanese
        - Spanish (MX) (eventually)
- Heal on Kill
    - Taking damage interrupts healing
- Kill streaks
- Dynamic stats
- Railings destroyed on round start
- AFK system

## Import Codes
- BKRXY (NA/EU)
- 5RKYY (JP)

