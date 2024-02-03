# Counter-Strike Version 1.5

## Supported versions
- [x] **Windows**
- [x] **Linux**

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.1.1.0
- Linux: Half-Life Dedicated Server v3.1.1.0
_____

# Changelog

```
v1.5
----
[6.12.02]

Changes/Additions :
-------------------
- New map de_piranesi.
- Ricochet included in this release.
- Added logging of the anti-cheat system catching and kicking detected cheats.
- Added logging of "kick" commands.
- Added logging of "banid" commands.
- Changed error message if clients try to download missing resources to be more helpful.
- Changed 'exec' command now only works on .cfg and .rc files.
- Changed 'exec' command no longer allows ".." or "\\" or ":" in the filename.
- Added new debug message for mod makers if a packet couldn't be parsed correctly.
- Linux: hlds_run now does auto-restart by default (to disable: define "-norestart" on the command line)
- Linux: hlds_run uses "exec" when you define the "-norestart" option.
- Linux: Added -pingboost command line parameter.  Currently supports three different methods ('-pingboost 1', '-pingboost 2', and 'pingboost 3').  These may not work well (or at all) on some OS environments.
- Linux: Added "-debug" flag to hlds_run to automatically run gdb and pull out useful info.

New CVARS:
----------
- Added "serverversion", can be set to '1108' to view/re-record old demos.
- Added "sv_logbans" to turn the logging of player bans on and off.  Default is 0 (off).

Bug Fixes:
----------
- Fixed mp_hostagepenalty not working.
- Fixed problem with server locking when the bomb is planted and a new player joins the server.
- Restored "mp_fadetoblack" server variable.
- Fixed incorrect WonID logging.
- Fixed sv_allowdownload being required to be set to 1 for clients to connect to secure servers.
- Fixed 'bad address type' fatal error on servers that attempt to run in secure mode but have no DNS resolution.
- Fixed DropClient messages for Steam clients who were banned or have a duplicate Steam ID to properly show the SteamID of the client.
- Fixed HLTV reporting wrong spectator numbers if connection to server was pending.
- Fixed "multicast 1" not working if it was issued before HLTV connected to game server.
- Fixed relay proxies reporting wrong spectator/slots numbers in multiplayer/LAN menu.
- Fixed DMC powerup bug where the invisibility ring would make people glow red.
- Fixed rcon bug in HLTV.
- Fixed delay being reset to default value during changelevel.
- Fixed a problem with propagating HLTV banners.
- Fixed client freeze on exit.
- Fixed framerate problem on some ATI video cards.
- Fixed MaxPing filter not being saved correctly.
- Fixed sky box bug.
- Fixed TFC spy disguise menu bug.
- Fixed DMC view model animation bug.
- Fixed bug using "exec <filename>" on large files (e.g. banned.cfg).
- Linux: Fixed server using 64 MB more memory than it needed to.
- Linux: Fixed 'undefined symbol: __strtouq_internal' on some Linux systems.
- Linux: Fixed segmentation fault on some Linux systems when attempting to run in secure mode.
```