# Counter-Strike Version 1.4

## Supported versions
- [x] **Windows**
- [x] **Linux**

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.1.1.0
- Linux: Half-Life Dedicated Server v3.1.1.0
_____

# Changelog

```
v1.4
----
[4.24.02]

Changes/Additions :
-------------------
- Added Anti-Cheat protection.
- User Interface redone for HLTV.
- Dedicated servers (Win32 + Linux) now default to 32MB heapsize.
- Improved dedicated server FPS (sys_ticrate) accuracy in Windows NT/2K/XP and Linux.
- New map cs_havana
- New map de_chateau
- Updated version of map de_train
- Enhanced in-game spectator mode to include HLTV features
- Added new first-person mode to spectator modes
- Speaking players flash in team members' radars
- Dead bodies remain on the ground for the entire round
- Dropped bomb blinks red in Terrorist team's radar
- Changed so only Terrorists are notified when the bomb is dropped or picked up
- Changed so players must stand still when planting the bomb (including no jumping)
- Changed so players can't move or shoot while defusing the bomb
- Adjusted pistol accuracy while jumping (all pistols)
- Adjusted player jumping values to minimize bunny hopping
- Changed so the VIP can't drop any weapons
- If player dies, view zooms away from falling body while changing the angle to show the killer
- Changed color of the words 'BOMB' and 'VIP' in the scoreboard to make them more visible
- Changed so name changes for dead players are stored and processed when the players respawn back into the world
- Changed the way "kevlar" and "kevlar/helmet" work using the buy menus...made them work together
- Added a sound when "kevlar" and "kevlar/helmet" are purchased
- Removed players hearing enemy radio calls
- Added code to force "sv_clienttrace 1" on the server
- Changed so when someone mutes a player (in the scoreboard), they will no longer see that player's in-game text messages either
- Added cheering to HLTV.
- Muting a player in the scoreboard will also mute their text messages.
- Steam beta clients and non-Steam clients can play together on the same server now.
- Voice communication uses DirectSound by default now.
- Added player ID to Half-Life DM.
- Added chat flood protection to HLDM.
- Added logging of fatal Sys_Error server shutdowns.
- Renamed setinfo items "ah" and "vgui_menus" to "_ah" and "_vgui_menus"
- Added new setinfo item "_cl_autowepswitch" (default: 1) which controls whether or not a client switches to picked up weapons (if they're more powerful)

New CVARS :
-----------
"mp_kickpercent"
sets the percentage of teammates it takes to vote off a player
maximum: 1.0
minimum: 0.0
default: 0.66

"sv_restart"
acts exactly the same as "sv_restartround"

"sv_send_logos"
when "sv_allowdownloads" is set to 1, this cvar will control whether custom logos are propagated to clients
default: 1

"sv_send_resources"
when "sv_allowdownloads" is set to 1, this cvar will control whether resources are propagated to clients
default: 1

"cl_corpsestay"
client-side cvar to set the amount of time (in seconds) dead bodies will stay before sinking into the ground.  Dead bodies are cleared at the beginning of each round.
default: 600

"cl_righthand"
client-side cvar to toggle using the right and left hand view-models
default: 1

"cl_minmodels"
client-side cvar so clients can play using the minimum model set: leet.mdl, gign.mdl, and vip.mdl
default: 0

Bug Fixes :
-----------
- Smoke grenade fix
- Radio command fix
- Fixed duplicate HUD weapon sprite bug
- Fixed footstep sounds to correctly play when not walking (fixes fastwalk cheats)
- Fixed uneven movement rate when moving through water
- Fixed server locking up at end of round when a lot of grenades are in play
- Fixed several ammo inconsistencies between weapons that share ammo types
- Fixed a T as CT skin bug
- Fixed bug with "kevlar/helmet" where players could buy it again at the beginning of each round even if they didn't need it
- Fixed some view_model animation bugs
- Fixed 'use' key causing an instant player stop with no deceleration
- Fixed bogus \Save directory being created when you ran Half-Life.
- Fixed filter logic in the launcher.
- Fixed bug where clients couldn't connect to server side only MODs.
- Fixed bug where you could "kill" the HLTV entity in Half-Life DM.
- Fixed AddIP command.
- Fixed crash when a func_breakable triggers a trigger_counter.
- Fixed Egon gun beam problem in Half-Life DM.
- Fixed Tau cannon prediction problem.
- Fixed fog messing Additive sprites.
- Fixed Alien Grunts not making any attack sounds.
- Fixed Egon's beam looking yellow in sofware mode.
- Removed "friends" connectionless packet query.
- Fixed "bad address type" fatal server error (caused by clients with long names).
- Fixed "condump" so the output won't overwrite previous files.
- Fixed "cvarlist" so the output won't overwrite previous files.
- Fixed rcon_port and rcon_address so they can be set manually by the player to rcon a server.
- Fixed server shutdowns related to using bots.
- Fixed "vote" and "votemap" commands to work correctly
- Fixed bug where clients would try to change their name while dead and then couldn't change it when they respawned.
```