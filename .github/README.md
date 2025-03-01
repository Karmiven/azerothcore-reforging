# ![logo](https://raw.githubusercontent.com/azerothcore/azerothcore.github.io/master/images/logo-github.png) AzerothCore

# Reforging System for AzerothCore

## Overview

First, thank you Rochet2 for inspiration. His reforging repo for TrinityCore can be found here: https://github.com/Rochet2/TrinityCore/tree/reforging_3.3.5/src/server/scripts/Custom/Reforging

Adds the possiblity to **reforge** items on 3.3.5a client. Reforging allows players to **decrease** a stat by a certain percentage (default is 40%) and **add** a new stat based on the difference. The allowed stats and the percentage is **configurable** via the mod .conf file.

## Limitations

1. Due to the nature of **WOTLK** client, the new **STATS** will only be visible to the owner. **This is only visual, stats will be there nonetheless!** 
2. Upgrades will be lost (of course) when trading, sending mail, depositing to guild bank, deposit to auction.
3. Heirlooms can't be reforged.
4. Items with random properties (like "of the Bear", "of Intellect") can't be reforged.

**WARNING**: this is **NOT** compatible with the **Individual item upgrades**: https://github.com/silviu20092/azerothcore-item-upgrades, although you can have both systems, if an item is **both** upgraded and reforged, the stats won't be calculated properly. The two systems are not aware of each other and will step on each other's foot as both systems try to alter item's stats.

## How to install

1. Clone this repository to your AzerothCore repo modules folder. You should now have mod-reforging folder there.
2. Re-run cmake to generate the solution.
3. Re-build your project.
4. You should have mod_reforging.conf.dist copied in configs/modules after building, copy this to your server's binaries folder.
5. Start the server, .sql files should automatically be imported in DB, if not, apply them manually.

WARNING: this mod requires at least this version of AzerothCore https://github.com/azerothcore/azerothcore-wotlk/commit/3988e9581d736f8c7891baaf13011e9df4f46fa4

## Ingame usage

Use .npc add 200004 to spawn the Master Reforger NPC. The rest is self explanatory.

## Some photos

![pic1](https://github.com/silviu20092/mod-reforging/blob/master/pics/pic1.jpg?raw=true)
![pic2](https://github.com/silviu20092/mod-reforging/blob/master/pics/pic2.jpg?raw=true)
![pic3](https://github.com/silviu20092/mod-reforging/blob/master/pics/pic3.jpg?raw=true)
![pic4](https://github.com/silviu20092/mod-reforging/blob/master/pics/pic4.jpg?raw=true)
![pic5](https://github.com/silviu20092/mod-reforging/blob/master/pics/pic5.jpg?raw=true)

## Credits
- silviu20092