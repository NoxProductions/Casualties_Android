# Casualties: Android
![Total Downloads](https://img.shields.io/github/downloads/NoxProductions/Casualties_Android/total)
![GitHub Stars](https://img.shields.io/github/stars/NoxProductions/Casualties_Android?style=flat-square&color=gold)
[![License](https://img.shields.io/badge/License-Custom-gold?style=flat-square)](LICENSE.txt)

> 💛 Like what I'm building? [sponsoring](https://github.com/sponsors/NoxProductions) goes toward updates, a multiplayer rework, and possible mod support.

> For bug reports ( in case you don't have a github account ), you can join my discrd [server](https://discord.gg/5TQcFMM54t)

This is an Android port of **Casualties Unknown**, with multiplayer built in so you can join **KrokMP**
co op games from your phone. Grab the APK from Releases, install it, open the Multiplayer menu, type a host's
IP, and you drop into their world together.

The multiplayer client speaks KrokMP's protocol natively, so it connects straight to a KrokMP host. Right now
it works with **KrokMP 4.0.1** hosts.

## Download and install

1. Get the latest APK from the **Releases** page.
2. On your phone, allow installing from unknown sources for your browser or file manager.
3. Open the APK and install it.
4. Launch the game.

## Playing multiplayer

This build is **local only**, you join a host by direct IP on the same network. There is no Steam lobby
browser in this version yet. Steam discovery is coming with **KrokMP 5.0.0**.

To join, open the Multiplayer menu, set your name and the host IP, then press **JOIN KrokMP**. The host needs
to be running KrokMP and hosting over direct IP.

Use the host PC's **IPv4 address**, not `127.0.0.1`. On the PC, open Command Prompt and run `ipconfig`, then
look for the IPv4 line under your active adapter, for example:

```
Ethernet adapter Ethernet:

   Connection-specific DNS Suffix  . :
   IPv4 Address. . . . . . . . . . . : 192.168.1.42
```

Type that address (like `192.168.1.42`) into the Host IP field. Both devices need to be on the same network,
and the PC may need to allow the game through its firewall on UDP port 7790.

## What works and what does not, until KrokMP 5.0.0

| Feature | Status |
|---|---|
| Join a KrokMP host by IP and appear in the player list | Works |
| Load into the host's world, terrain matches the host | Works |
| See other players as real characters, moving, with nametags and colours | Works |
| Your movement shows up on the host so others see you move | Works |
| Carry and piggyback, both directions, with correct facing | Works |
| Water and fluid sync | Works |
| Health sync, you can see wounds and the host can pull shrapnel or fix dislocations on you | Works |
| Loot spawns and syncs, loose items, crates, corpses, command spawned creatures | Works |
| Pick up, drop, and move items between inventory slots, both directions | Works |
| Held and worn items show on other players | Works |
| Keypad and lockpick minigames sync, you can unlock crates with the host's code | Works |
| Using and eating items reaches the host in most cases | Works |
| Attacks, hitting buildings and breaking blocks reach the host | Works |
| Block damage from other players shows up on your screen | Works |
| In game multiplayer panel with the roster, names, colours, and pings | Works |
| See Health Panel button for a nearby player, shows their name and vitals | Works |
| Return to the lobby or menu when the host saves and quits | Works |
| Cheat command gate, you can only run cheat commands if the host allows it | Works |
| Steam lobby discovery, joining the public lobby list | Coming in 5.0.0, this build is local only |
| Eating food off the floor on your phone clearing it on the PC | Does not clear, kept as a gimmick for now |
| Healing another player from their health panel | View only for now |
| Seeing other players' hands during a shared minigame | Not yet |
| Starting medical minigames on other players from your phone | Not yet |
| Seeing a full inventory of another player beyond what they hold or wear | Not yet |

## Known quirks, cosmetic only

* On the other player's screen, your character's facing is sometimes mirrored or stuck. Your own view and all
  gameplay are correct, it is only how you look to them.
* Some non networked decor, like cave hole light and glow plants, can differ between screens.
* Creatures move and attack correctly but their animation is not fully synced.

## Differences from the PC version

This is a port, so a few things are not one to one with the PC build.

* Visuals are not identical due to an upgrade in shaders.
* Performance on lower end phones is acceptable, a Pixel 4a ( 2020 ) can run it at about 60fps on average in sandbox mode, 30-40fps in WorldGen.

## Compatibility

**All Mali GPU's are now mostly supported!**

* Phone brands likely supported: Pixel ( Pixel 6 and newer / Tensor models ), Xiaomi ( Mid-Range & Upper Mid-Range ), Redmi ( Budget & Mid-Range ), Poco ( Select Mid-Range ), Realme ( Budget & Mid-Range ), Oppo ( Mid-Range & Flagship ), Vivo ( Mid-Range & Flagship ), OnePlus ( Mid-Range & Upper Mid-Range ), Samsung ( Galaxy A-series & Select FE ), Motorola ( Budget & Mid-Range ), Tecno ( Budget & Mid-Range ), and Infinix ( Budget & Mid-Range ).

* Phone brands fully supported: Pixel ( Pixel 5a and older / Snapdragon models ), Samsung ( Mid-Range & Flagship ), Xiaomi ( Mid-Range & Flagship ), OnePlus ( Mid-Range & Flagship ), iQOO ( Mid-Range & Flagship ), Poco ( Mid-Range & Upper Tier ), Realme ( Mid-Range & Upper Tier ), Motorola ( Mid-Range & Flagship ), Sony ( Flagship ), Asus / ROG ( Flagship ), RedMagic ( Flagship ), and Nothing ( Mid-Range & Upper Mid-Range ).

## Credits

* **[Orsoniks](https://github.com/Orsoniks)**, for making Casualties Unknown, the game this is built on.
* **Noxbit**, for the Android and Multiplayer port.
* The multiplayer connects to **[KrokMP](https://github.com/creaturefeaturelarry/casualties-together)** (Krokosha's Casualties Together co op mod), which is what the host runs.
* [**NotTheBadGuy**](https://github.com/notthebadguy), for play testing Casualties: Android and reporting bugs.

## Notes

KrokMP 5.0.0 is a full remaster of the mod's sync and it will change how hosting and joining work, including
Steam discovery. Expect a new APK once that lands. Until then this is the local only version, meant to be
played with friends over direct IP.
