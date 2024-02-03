# Counter-Strike Version 1.1 

## Supported versions
- [x] **Windows**
- [x] **Linux**

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.1.1.0
- Linux: Half-Life Dedicated Server v3.1.1.0
_____

# Changelog

```
v1.1
-----
[3.13.01]

Changes/Additions:
------------------
- Added spectator mode -- allow_spectators (0/1)
- Terrorist bomb backpack re-added
- Upgraded player models to 512X512 textures
- CT defuse kit pack re-added
- Made jumping while shooting more inaccurate w/ submachineguns
- Took out sniper crosshair when zoomed out
- AWP leg shots now non-lethal
- Swimming animation added to models
- Status bar text uses team colors
- All CS Strings localized to titles.txt
- Added option to take "end game" screenshot
- Length of MOTD increased to 1536
- Added cs_thunder, de_vertigo, de_inferno, de_dust2 & de_rotterdam
- Upgraded de_dust de_cbble, de_vegas, de_aztec, cs_office, cs_siege, & cs_italy
- Logic used to cycle the map has been changed.  The map will cycle if
  one of three conditions has been met: "mp_timelimit" has been met,
  "mp_winlimit" rounds have been won by one of the teams, or "mp_maxrounds" 
  have been played.
- Fixed many cheats
- Changed logging format to meet the standars @:
  http://www.hlstats.org/logs/
	Several events have been added to the logs:
	a) "Begin_Bomb_Defuse_Without_Kit"
	b) "Begin_Bomb_Defuse_With_Kit"
	c) "Spawned_With_The_Bomb"
	d) "Dropped_The_Bomb"
	e) "Got_The_Bomb"
	f) "Became_VIP"
	g) "Escaped_As_VIP"
	h) "Round_Start"
	i) "Round_End"


Bug Fixes:
----------
- "Out of ammo" hint message fixed
- "Punished for tk" hint message fixed
- "Through floor" death animation fixed


New/Changed CVARS:
------------------

mp_playerid 
Toggles what information players see in the status bar
0 everyone: players see all names listed in the status bar (with appropriate
team colors)
1 team only: players only see names for their teammates and hostages in the
status bar
2 off: players do not see any names in the status bar (hostages included)
0 is the default


mp_fadetoblack (overrides mp_forcechasecam)
0 nothing
1 player's screen fades to black for the remainder of the round when he dies
(hud still works normally so player can chat and see the scores, etc.)
0 is the default


mp_forcechasecam
0 free to spectate anyone when player dies
1 only allowed to spectate player's own team when player dies
2 not allowed to spectate anyone...player's view stays where the player dies
0 is the default


mp_buytime (float)
Can now designate the desired amount of buy time for each round
min buy time is .5 minutes
no max buy time
Example: mp_buytime 1.8   // 108 seconds of buy time
1.5 min is the default (CS 1.0 buy time)


mp_roundtime (float)
Changed to support partial minutes
min round time is 1 min
max round time is 9 min
Example: mp_roundtime 1.3   // 78 seconds
5 min is the default (CS 1.0 round time)


mp_winlimit
Will cycle the map after one team reaches this many wins 
0 is the default (no win limit)


mp_timelimit (float)
Fixed to support 0 (no time limit)
Example: mp_timelimit 17.2   //  17 minutes 12 seconds
0 is the default


allow_spectators
0 Do not allow spectators
1 Allow spectators
```