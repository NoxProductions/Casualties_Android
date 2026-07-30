# Casualties Unknown, Android Port with Multiplayer

This is an Android port of **Casualties Unknown**, with multiplayer built in so you can join real **KrokMP**
co op games from your phone. Grab the APK from Releases, install it, open the Multiplayer menu, type a host's
IP, and you drop into their world together.

The multiplayer client speaks KrokMP's protocol natively, so it connects straight to a KrokMP host. Right now
it works with **KrokMP 4.0.1** hosts.

## Download and install

1. Get the latest APK from the **Releases** page.
2. On your phone, allow installing from unknown sources for your browser or file manager.
3. Open the APK and install it.
4. Launch the game, it runs offline as a single player game too.

## Playing multiplayer

This build is **local only**, you join a host by direct IP on the same network. There is no Steam lobby
browser in this version yet. Steam discovery is coming with **KrokMP 5.0.0**.

To join, open the Multiplayer menu, set your name and the host IP, then press **JOIN KrokMP**. The host needs
to be running KrokMP and hosting over direct IP.

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

* Visuals are not identical. The shaders were rebuilt from scratch and some effects were simplified for
  performance, so lighting and certain effects can look a little different from the PC version.
* The depression music is not one to one effect wise. It is supposed to have an echo, that was removed for now,
  and it comes back in the 5.0.0 update.
* Performance on lower end phones is still rough. The 5.0.0 update brings more optimization so lower end devices
  can run it above 10 fps.

## Credits

* **Orsoniks**, for making Casualties Unknown, the game this is built on.
* **Noxbit**, for the Android port and the multiplayer, about a month of work.
* The multiplayer connects to **KrokMP** (Krokosha's Casualties Together co op mod), which is what the host runs.

## Notes

KrokMP 5.0.0 is a full remaster of the mod's sync and it will change how hosting and joining work, including
Steam discovery. Expect a new APK once that lands. Until then this is the local only version, meant to be
played with friends over direct IP.
