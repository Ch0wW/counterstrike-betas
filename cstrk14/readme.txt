______________________________________
Counter-Strike Mod for Half-Life
v1.4 Release Documentation -- Readme.txt
http://www.counter-strike.net
______________________________________


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


v1.1c
-----
[4.6.01]

Bug Fixes:
----------
- Incorrect Hitboxes fixed when holding specific weapons.

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









v1.0
-----
[11.8.00]
- added three new weapons:
  (H&K UMP .45, FN Five-Seven, & SIG SG-550)
- redone player models
- incorporated Valve's model blending technology
- left beta stages



BETA 7.1
--------
[9.13.00]

- fixed de_vegas crashing
- tweaked burst fire accuracy system
- slightly improved vehicle code
- included missing skies (for cs_arabstreets, de_train)
- fixed mp_timelimit bug
- added APC to cs_siege
- new server variable, "mp_maxrounds X"   {X = maximum number of rounds to be played on a map, 
if X = 0, then maps will rotate based on mp_timelimit}
- fixed crosshairs {They now expand regardless of lag}
- fixed player heights {Player's POV is now representative of the third person player model}
- fixed shotgun not showing up in VGUI menus in as_ maps for CTs
- included new death icon for headshots



BETA 7.0
--------
[8.26.00]

- added dual Berettas
- added redone Knife Model (added a secondary attack mode for knife)
- fully implemented VGUI
- added new player model (Seal Team 6)
- added several new player animations
- fixed locked chasecam
- gave VIP a USP
- added cs_office, as_highrise, cs_arabstreets, de_foption & de_vegas
- fixed many bugs & exploits
- added driveable vehicle support
- added driveable vehicle test map de_jeepathon2000

New Commands:
------------

setinfo vgui_menus X  
{X = 0 or 1,  0 disables VGUI menus, 1 enables VGUI menus}
(also available through the "Play CS" > "Customize" menu)

*Note: If the buy weapon system malfunctions, disable the vgui
through the "Play CS" > "Customize" menu

*Note: de_jeepathon2000 is meant as a test/prototype map only.






BETA 6.6
--------
[6.22.00]

- added new command 'timeleft'
- fixed stalled connection bug
- new sniper crosshair
- fixes "laggy rifle firing"
- fixed many cheats
- updated cs_estate

New Commands:
------------

timeleft
{tells you how much time is left on the map}



BETA 6.5
--------
[6.8.00]

- Integrates Valve's rewrite of the HL networking system
- Added Smoke Grenade
- Added "Gorilla Warface" player model
- Redone models for .45 USP, M3,  SG-552, and Colt M4A1 
- Added more realistic smoke f/x, and shell ejection
- Added Valve's Chasecam modes (roam, free, and locked)
- Integrates Nighthawk's Model Bounds Checker algorithm
- Added as_forest.bsp, de_cbble.bsp, de_aztec.bsp, as_tundra.bsp, cs_italy, es_trinity, cs_estate
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
X = max. number of hostages you can kill before the server boots you out... 
setting this to 0 will shut off this command

mp_logmessages  0/1   
used for server admins to spit out chat messages in their log files

mp_forcechasecam  0/1
Setting this to 1 will force chasecam to be teammate only
(useful for LAN games)





BETA 6.1
[server side only]
--------
[3.24.00]
- off center shooting fixed
- greatly improved nightvision
- can buy nightvision using the 'buyequip' command
- ammo bugs fixed
- 120 round limit for the mp5 and tmp
- prisoners are notified when someone escapes
- draw games eliminated, now scenario specific
- new TK 1 round "time-out" penalty 


BETA 6.0
--------
[3.10.00]

- added MAC-10 weapon
- added Steyr Aug weapon
- added new gametype: Assassination (as_x)
- added new gametype: Escape (es_x)
- added right and left handed weapons
- added new radar tracking for teammates
- re-added Night Vision Goggles
- added new Terrorist Snow player model
- added new CT French GIGN player model
- tweaked player speeds / acceleration
- added new radio commands
- redone mp5 model / animations
- added maps de_fang, es_jail, es_frantic,
  as_oilrig, as_riverside, cs_747
- updated previous maps



Misc 6.0 Notes:
---------------
Assassination Gameplay: One member of the CT team will serve as the VIP.
The object is to get the VIP safely to the pre-defined escape points. If he
dies, the CT's lose the round. If he makes it safely, the CT's win. VIP has
a unique skin, only carries a knife, and has ample body armor. Certain
weapons cannot be purchased by each team in this gameplay scenario.

Escape Gameplay: The T team starts out in a fortified location and must
"escape" to one of the pre-defined escape points. The CT's must exterminate
them before they can escape. The T's win the round once 50% of the team has
successfully escaped. They can also break into the armory to steal weapons,
or just get out of there. The two teams will switch roles after every 8
rounds of play.

After buying NVG, you toggle it on/off by using the "nightvision" command. Be
warned that the NVG will not be effective on every hardware setup. It may or not
work well for you.

To switch between right and left hand weapons, go to:
multiplayer > Customize > Advanced Options
There will be a checkbox for you to select the hand of your choice.








BETA 5.2
--------
[1.10.00]

- Fixed crashing bugs 
- Implemented a new lower bandwidth chasecam
- Prevented players from changing name when they're dead
- Fixed scoreboard not showing 20 players
- Show scoreboard at the end of the map rotation



BETA 5.0
--------
[12.23.99]

New Content:
- Added Benelli XM 1014 fully automatic shotgun
- New Hostage model and two new skins.
- SAS model added as a selectable CT
- Added maps cs_backalley and de_train
- Updated maps cs_station, de_nuke, de_dust, and de_prodigy
- New icons for HUD (money, weapons, armor, timer, C4, defuse Kit, scoreboard)
- Added buy zones, reload zones, hostage, and bomb target zones to HUD.
- an extensive help manual located at \half-life\cstrike\manual\index.htm.
- Verbose Auto-help
- added auto-id

Gameplay Changes:
- C4 is now an equipment item in slot 5 (to plant, select then hold down fire)
- C4 can only be planted in bomb delivery zone
- To defuse a bomb Counter Terrorists must target C4, press and hold the USE key
- CTs can defuse C4 without a defuse kit in 10 seconds
- CTs can defuse C4 with a defuse kit in 5 seconds 
- A progress meter is added showing CTs their progress defusing a bomb
- A progress meter is added showing Ts their progress planting a bomb (this takes 3 seconds)
- Defuse kit now an item which can be purchased - Nobody starts with a defuse kit
- Defusing bomb wins round for Counter Terrorists
- C4 can be dropped for other teammates
- Hostages are automatically rescued at hostage rescue zones
- Counter Terrorist and Terrorist teams are now labeled
- Individual frags can be toggled on or off
- Ghosts can be made visible to other ghosts (client defined)
- Pre-Round grace timer standard setting 6 seconds (server defined)
- Three observer modes: classic ghost, locked chasecam and freelook chasecam ( press jump to toggle)
- Auto-find teammate in observer mode (primary fire)
- New radio messages and organization of radio keys (standard, group and report messages)
- Can hear other players reloading
- Mission briefing added to maps (can also be invoked during round)



BETA 4.1
--------
[12.1.99]

[server side only release]
-team chat while dead works
-icon mixup for bomb/defuser fixed
-slightly less money given to losers
-allow Ts to pick up C4 if it's not planted in the proper spot (crouch)
-default C4 timer to 35 seconds
-toned down P228
-prevent players from buying stuff when they're dead by using aliases
-accuracies tweaked



BETA 4.0
--------
[11.5.99]

- Added Sig P228 pistol, and Steyr Scout sniper rifle
- Added new gameplay scenario involving C4 bombs
- tweaked firing system for all guns
- added High-Explosive (HE) grenades
- modified hostage rescue scenario (rescuing 50% of the hostages will result in a CT win)
- modified kick vote system (only 65% of a team is needed to kick vote someone off)
- loose guns are removed at the start of a round. (no more gun running)
- loser bonuses are increased to allow the losing team to stand a fighting chance
- altered money bonuses for rescuing hostages :
- added cs_station, de_nuke, de_dust, de_prodigy
- modified cs_ship, cs_siege, cs_docks, cs_tire, cs_facility
- automatic flashbang .wav added back
- new, closer rescue points added to cs_ship, cs_siege, cs_tire
- new ammo system, primary and secondary (less mind boggling)



BETA 3.1
--------
[9.16.99]

- Bullet penetration bug fixed
- Radio .wav's now have lower volume
- Removed automatic .wav's (death, flashbang)
- fixed MRAD_ENEMYSPOTTED error
- Disorientation system changed
- Added "ignoreradio" command to only ignore .wav's
- Flashbang Shrapnel altered



BETA 3.0
--------
[9.14.99]

- Added a knife weapon for those last resort situations
- Added a kevlar+helmet combination
- *GREATLY* improved hostage path AI
- Added concussion grenades which shoot out shrapnel as well as a bright flash
- Added a new weapon, the Fabrique Nationale P90 submachine gun
- Added a radio system
- Modified the scoreboard
- modified the shotgun



BETA 2.1
--------
[8.17.99]

- added new vesion of cs_assault (compatible w/ hlserver.exe)
- added scientist model for hlserver.exe
- added assault's proper sky
- fixed telefragging  (cs_alley will no longer telefrag)
- fixed dropweapon
- fixed those spurious 'player joined' messages
- changed Ak-47 price



BETA 2.0
--------
[8.13.99]

NEW Features :
- Three new guns added : {Sig SG-552 Commando , AK-47 , Desert Eagle}
- Added silencers to the USP .45 Tactical and the Colt M4A1
- Added a round timer which shows how much time is left in the round
- Added team scores which shows how many rounds a team has won
- Added Night Vision Goggles
- Added new entity for mappers to use (info_hostage_rescue)
- Optimized all the models for lower r_speeds!
- Ability to assign keys to all of the commands from the controls menu  
  (courtesy of cannelbrae of Gunman project)



BETA 1.2
--------
[7.20.99]

- 5 second "molasses period" at the start of all rounds to dissuade rushing tactics 
- kick option added
- Refined the prices for some of the gunS
- made the kevlar MUCH more effective (it now covers people's arms) 
- made jumping and shooting MUCH more inaccurate for all the guns
- added a $16,000 salary cap 
- tweaked the bonus money awards. 
- tweaked the flashbangs effectiveness



BETA 1.1
--------
[6.27.99]

- greatly improved server stability, crashes should be eliminated
- primary servers will now work with CS
- fixed the ammo and armour reset bugs
- balanced the economic system a bit
- added new firing mode for the glock18
- enabled 'mp_friendlyfire' command for server admins
- fixed map rotation
- adds two new maps: cs_assault & cs_desert
- cs_siege fixes
- cs_wpndepot fixes



BETA 1.0
--------
[6.19.99]
Features :

- weapons: usp, glock, shotgun, m4a1, mp5 navy, TMP, awp, G3/SG-1 & FN M249 PARA 
- hostage rescue scenario
- custom maps: cs_siege, cs_mansion, cs_wpndepot, cs_prison



-------------------------------------------------------------



Counter-Strike is a modification (MOD) to the excellent game, Half-Life. 
It modifies the multiplayer aspects of Half-Life to bring to it a more team-oriented 
gameplay. Not terribly unlike Team Fortress 2, Counter-Strike provides the player 
with an experience that a trained counter-terrorist unit or terrorist unit experiences.
 
The MOD is team-based featuring one team playing the role of the terrorist and the other 
team playing the role of the counter-terrorist. Each side has access to different guns and 
equipment, as well as different abilities. Maps have have different goals such as: hostage rescue, 
assassination, bomb defusion, Terrorist escape, etc. 

Weapons include the usual assortment of pistols, shotguns, assault rifles, sniper rifles, grenades, 
demolition devices. Each side has access to a different subset of weapons so for example only the 
counter-terrorist can use the M4A1, and only the terrorists can use the AK-47.

We are confident that we've created a MOD quite unlike any other. We hope you will be immersed in
the frightening and intense world of Counter-Terrorism.






------------------ credits ---------------------------------


THE CS TEAM
-----------


Gooseman
gooseman@counter-strike.net 
Project leader, Head modeler, Head coder, Head-job



cliffe
cliffe@counter-strike.net 
2d-graphics, sound effects, QA, PR, jack of all trades, etc.




(Mappers):
------------


de_survivor
by 3d_Mike
3D_Mike@soneramail.nl

de_torn
by Crinity & Madcross
crinity@email.com

de_storm
by Daank
daankvirus420k@icqmail.com

de_inferno
by Barney (aka Narby)
fragged101@yahoo.com

cs_italy
by DigiChaos
& GlenC

as_tundra
by Zaphod Beeblebrox
coyote@eudoramail.com

cs_estate
by Zaphod Beeblebrox
coyote@eudoramail.com

as_oilrig
by MacMan 
macmaninfi@aol.com

cs_backalley
by TYR 
tyr@barking-dog.com

de_aztec
by Barney (aka Narby)
fragged101@yahoo.com

de_vegas
by Cadaver
mlr32@cam.ac.uk

de_train
by Chris Mair
chris@barking-dog.com

cs_militia
by Andrew Aumann
andrewja@home.com

cs_747 
by Markus
witchdawn@hotmail.com

cs_docks
by N0TH1NG
N0TH1NG@mailcity.com

cs_siege
by N0TH1NG
N0TH1NG@mailcity.com

cs_assault 
by CryptR 
lmuur@dlc.fi

de_dust
by Davej
dv@btinternet.com

de_cbble
by Davej
dv@btinternet.com

de_prodigy
by Hobbit
hobbit@bellatlantic.net

cs_office
by Hobbit
hobbit@bellatlantic.net

de_nuke
by MEEEEDIC
jogi@netads.de


The texture Artists:
--------------------

Chris Ashton (aka Macman)
MacManInfi@aol.com

Ido Magal
ido@dnai.com 



Splash and Console 2d Art:
--------------------------
Cliffe


High Quality Shell:
------------------
John "Rizzuh" Jensen


CS icon by:
-----------
Greg Fleming
Dark Project Studios
www.darkproject.com


Special Thanks:
---------------

Thanks to:
----------

Mr_Grim			: for his help in coding the radio system, and other things
BETA test team	        : for helping us test.. and for providing the occasional premature leak
Valve Software	        : for their constant support
Fanny			: for giving Gooseman motivation!
David "Nighthawk" Flor  : for the Model Bounds Checker algorithm
Mappers, Texture artists


Extra special thanks to:
-----------------------
Ben Wilder <wilder@cleanweb.net>
Programming to mirror the weapons to the right hand


Also thanks to:
---------------
Gabe Newell; Gamespy Industries; Oddjob, Mr. Grim, and Dallas Frank of the A-Team;  
MTG; Poor Yurik; Brent Bussey; Valve Software; Art Min; Stikky & Adrian @ Gameplay;
Lestat, BizzyBlaster; D0gzilla; Chris Mair; Barking Dog Studios; Gamefan Network; 
Mutated Jellyfish; Gameplay.com; Darkman; TeamGT; Justin Bunnell,  Erik Johnston @ Valve; 
Leon Hartwig;  shirow @ mod central; Geronimo; RzE; MatteusX; John Jensen; Mr. Fraggle;
Frank Nuccio; Speakeasy.net;  Yahn Bernier; Macman; Jason Malhavoc Nugent; Redwood; Jcal;
Stomped.com; Art Min; Tactic; Stem; Darren Tabor; and the CS players. 

---------------





See manual.htm in your cstrike/manual directory for a full listing
of commands and documentation.




---------------------



Don't forget to visit the other sites on the Counter-strike.net network!

The Official CS Web Site
http://www.counter-strike.net/

CSNation
http://csnation.counter-strike.net/

CS Crossfire
http://crossfire.counter-strike.net/

CS Art
http://art.counter-strike.net/

CS Radio
http://csradio.counter-strike.net/

Counter-Server
http://server.counter-strike.net/

Z_Malloc Overflow
http://zmalloc.counter-strike.net/

Bots @ CS.net
http://bot.counter-strike.net/





--readme.txt by cliffe
e-mail cliffe@counter-strike.net


