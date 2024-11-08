# Counter-Strike Beta 6.5d

## Supported versions
- [x] **Windows** (v6.5)
- [x] **Linux** (v6.5d)

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.0.1.6 
- Linux: Half-Life Dedicated Server v3.0.1.6
_____

# Changelog

```
BETA 6.5d
[??.??.??]
- Advanced model checking to keep cheaters out
- Linux server bug of not being able to hear other players' footsteps fixed
- Faster load times
- Fixed connection problems
- Fixed gun-jamming


BETA 6.5
--------
[6.5.00]

- Integrates Valve's rewrite of the HL networking system
- Added Smoke Grenade
- Added "Gorilla Warface" player model
- Redone models for .45 USP, M3,  SG-552, and Colt M4A1 
- Added more realistic smoke f/x, and shell ejection
- Added Valve's Chasecam modes (roam, free, and locked)
- Integrates Nighthawk's Model Bounds Checker algorithm
- Added as_forest.bsp, de_cbble.bsp, de_aztec.bsp, as_tundra.bsp, cs_italy
- Added map voting system
- Updated maps


New Map Voting System:
---------------------

players type 'listmaps' to see the maps available to vote on, and then they type 
'votemap X'      where X is the corresponding number of the map.

Server admins who want to add new maps must also 
add an entry into mapcycle.txt,  that allows players 
to vote on any new maps.


New 6.5 Commands:
-----------------

fastsprites X    
x = 0   : regular transparent smoke grenade sprites
x = 1   : simple transparent smoke grenade sprites
x = 2   : VERY simple transparent smoke grenade sprites

max_shells   X         
X = maximum number of shells at one time

max_smokepuffs   X       
X = max. number of smoke puffs at one time

mp_tkpunish  0/1       
if set to 1, TK'ers will sit out next round

mp_hostagepenalty   X       
X = max. number of hostages you can kill before the server boots you out... setting this to 0 will shut off this command

mp_logmessages  0/1   
used for server admins to spit out chat messages in their log files

mp_forcechasecam  0/1
Setting this to 1 will force chasecam to be teammate only
(useful for LAN games)
```