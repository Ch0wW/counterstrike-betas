# Counter-Strike Version 1.3

## Supported versions
- [x] **Windows**
- [x] **Linux**

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.1.1.0
- Linux: Half-Life Dedicated Server v3.1.1.0
_____

# Changelog

```
v1.3
----
[9.12.01]

Changes/Additions:
------------------
- Multicast spectator added.
- Voice communication added.
- Added server chat to logging.
- Redesigned multiplayer scoreboard.
- CapsLock key is now bindable.
- Switching to Spectator is now logged.
- Changed minimum value for "mp_chattime" to 1 second
- Changed minimum value for "mp_buytime" to 0.25 (15 seconds)
- Radio commands can be heard by nearby enemies.
- Commandmenu support implemented.

New CVARS :
-----------
"mp_logdetail"
Bitwise cvar to set the level of detail for logging attacks.
Bit 0  - Log Enemy Attacks
Bit 1  - Log Teammate Attacks
default: 0
Usage:
"mp_logdetail 0"   - Log no attacks
"mp_logdetail 1"   - Log enemy attacks
"mp_logdetail 2"   - Log teammate attacks
"mp_logdetail 3"   - Log enemy AND teammate attacks

"mp_startmoney"
Sets the amount of starting money players may have.
maximum: 16000
minimum: 800
default: 800

Bug Fixes :
-----------
- Bunny hopping removed.
- Fixed client-side shots not matching the server-side counterparts.
- Fixed banned.cfg problem with more than 1024 entries.
- Fixed screenshots overwriting each other.
- Buffer overflow exploit fixed.
- "condump", "cmdlist", and "cvarlist" only write out to the game directory.
- Fixed Spectator mode bug.
- Fixed hitbox issues.
- Fixed nightvision bug.
- Fixed "slot10" not working correctly.
```