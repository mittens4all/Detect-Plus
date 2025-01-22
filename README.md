# Detect Plus

This behavior pack uses scripts to detect the player's selected slot on the hotbar and convert it to a scoreboard objective.
It also detects if the player is holding anything in mainhand or has any items in inventory and assigns it to scoreboard objectives.

## Installing the pack:

Add the Detect Plus add-on to your behavior packs on your world. Behavior packs disable achievements, but editing the world with an NBT editor can re-enable achievements when uploading your world to a realm.

Re-enable achievements on either pc or mobile with the free NBT editor [Dovetail](https://github.com/Offroaders123/Dovetail)

## How to Use

You can display the scoreboard objective `detect_air`, `detect_empty`, or `detect_slot`. 
You can also target players using the scores as part of the target selector arguments:
```js
execute as @a[scores={detect_air=1}] at @s run say you are holding air!

execute as @a[scores={detect_empty=1}] at @s run say you have no items in your inventory!

execute as @a[scores={detect_slot=1}] at @s run say you have selected the first hotbar slot!
```
- `detect_air`
Score of 1 means the player is not holding anything in mainhand.
Score of 0 means the player is holding a block/item in mainhand.
- `detect_empty`
Score of 1 means the player does not have anything in inventory.
Score of 0 means the player does have blocks/items in inventory.
- `detect_slot`
Score values range from 1 to 9 of the selected hotbar slots.

## Author

- [@mittens4all](https://www.github.com/mittens4all)
- [Youtube](https://www.youtube.com/@mittens4all)

## Gratitudes

- [JustAsh](https://github.com/Justash01)
- [Moriarty (ruandev)](https://www.youtube.com/@rmmrty)
- [Bedrock Add-Ons Discord](https://discord.gg/46JUdQb)

```js
       _                              _     _       _ _  
      (_)  _     _                   | |   (_)     | | | 
 ____  _ _| |_ _| |_ _____ ____   ___| |_____ _____| | | 
|    \| (_   _|_   _) ___ |  _ \ /___)_____  (____ | | | 
| | | | | | |_  | |_| ____| | | |___ |     | / ___ | | | 
|_|_|_|_|  \__)  \__)_____)_| |_(___/      |_\_____|\_)_)
                                                         
```