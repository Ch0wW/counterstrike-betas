______________________________________
Counter-Strike Mod for Half-Life
Beta5.0 Release Documentation -- Readme.txt
http://www.counter-strike.net
______________________________________

BETA 5.2
[1.10.00]

- Fixed crashing bugs 
- Implemented a new lower bandwidth chasecam
- Prevented players from changing name when they're dead
- Fixed scoreboard not showing 20 players
- Show scoreboard at the end of the map rotation

BETA 5.0
[12.23.99]

Beta 5.0 ships with an extensive help manual located at \half-life\cstrike\manual\index.htm.  Please refer to it for more extensive help.

New Content:
- Added Benelli XM 1014 fully automatic shotgun
- New Hostage model and two new skins.
- SAS model added as a selectable CT
- Added maps cs_backalley and de_train
- Updated maps cs_station, de_nuke, de_dust, and de_prodigy
- New icons for HUD (money, weapons, armor, timer, C4, defuse Kit, scoreboard)
- Added buy zones, reload zones, hostage, and bomb target zones to HUD.

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

Context Sensitive Help System:
Terse Auto-help
- Round start notification (i.e. hint to purchase items)
- Observer mode notification

Verbose Auto-help
- What to do with hostages (CTs rescue, Ts protect)
- What not to do with hostages (injuring/killing)
- How to lead hostages
- Looking at a friend for the first time
- Looking at an enemy for the first time
- What not to do with friends (injuring/killing)
- What to do with enemies (win by killing all enemies)
- Picking up C4 for the first time
- Out of ammunition for the first time
- In a bomb target zone for the first time
- In a hostage rescue zone for the first time
Auto-ID
- Friend (name and health displayed)
- Enemy (name displayed; health displayed only if observing)
- Hostage (health displayed) 

Map Credits:
------------

Hostage Rescue Maps:

cs_militia
by Andrew Aumann
andrewja@home.com

cs_station, 
by Markus
witchdawn@hotmail.com

cs_bunker
by Matthew Van Sickler 
mvsickler@uswest.net

cs_docks
by N0TH1NG
N0TH1NG@mailcity.com

cs_siege
by N0TH1NG
N0TH1NG@mailcity.com

cs_ship
by Poor Yurik 
yak@lvcm.com

cs_facility
by Captain Gram 
gram@bz2.com

cs_assault 
by CryptR 
lmuur@dlc.fi

cs_tire
by Davej (Curtains)
dave@3dgaming.com

cs_iraq
by Mr_Deth and Zaphod Beezlebub

"Defusion" C4 Bombing Maps:

de_dust
by Davej (Curtains)
dave@3dgaming.com

de_prodigy
by Hobbit
hobbit@bellatlantic.net

de_nuke
by MEEEEDIC
jogi@netads.de


BETA 4.0
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
   $500 for touching a hostage
   $1000 for successfully rescuing a hostage
   $500 team bonus
- added cs_station, de_nuke, de_dust, de_prodigy
- modified cs_ship, cs_siege, cs_docks, cs_tire, cs_facility
- automatic flashbang .wav added back
- new, closer rescue points added to cs_ship, cs_siege, cs_tire



****** What's new in BETA 4.0 ********

** New server variables :
 mp_roundtime X    {X is the number of minutes the round lasts. Valid values range between 3 and 9. Default is 5}
 mp_c4timer X      {X is the number of seconds the C4 bomb is set to blow. Valid values range between 10 and 90. Defaults is 30}
 mp_limitteams 0/1 {1 will restrict the number of players per team. Default is 1}
 mp_lowlag 0/1     {0 will causes more bullet sparks to be spawned, thereby creating more lag. Default is 1}
 mp_friendly_grenade_damage 0/1   {1 will result in HE grenades hurting teammates. Default is 1}

** New client commands :
 +showfrags        {displays every player's frag counts on the scoreboard}
 -showfrags        {only displays the player's frag count on the scoreboard}
 radio1            {brings up a list of radio commands}
 radio2            {brings up another list of radio commands}
 plant_c4          {plants the c4 bomb, if the player has one}
 
 
***** "Defusion" C4 bombing description *****

If a map has a target to be bombed, the terrorist team leader will be equipped with a C4 bomb. His goal is to plant the bomb at
the defined bomb target (marked on the map by a red target decal). Once the bomb has been planted, the bomb will blow up in X
seconds (where X is the server defined C4 timer variable, default at 30 seconds). The bomb will make an increasingly louder 
beeping sound as it nears the detonation time. After the bomb has been planted, any Counter-terrorist player equipped with a bomb
defuser may defuse the bomb by crouching on top of the bomb for 5 seconds. If the bomb goes off and the target is hit, the round will
end and the Terrorists will win. If the bomb has been planted and all the terrorists are eliminated, the round will not end until
the bomb has either been defused (CT wins) or detonated (Terrorist wins). A bomb's blast radius is fairly substantial and it's wise
to give yourself 10 seconds to run away from the bomb once it's been planted.

NOTE : Only half the CT team is equipped with bomb defusers.. It is recommended that this half of the team stay near the bomb targets
to listen for any beeping sounds.

Deufusion maps are denoted by de_mapname


____________________________________________________




Map Credits:
------------

Hostage Rescue Maps:

cs_militia
by Andrew Aumann
andrewja@home.com

cs_station, 
by Markus
witchdawn@hotmail.com

cs_bunker
by Matthew Van Sickler 
mvsickler@uswest.net

cs_docks
by N0TH1NG
N0TH1NG@mailcity.com

cs_siege
by N0TH1NG
N0TH1NG@mailcity.com

cs_ship
by Poor Yurik 
yak@lvcm.com

cs_facility
by Captain Gram 
gram@bz2.com

cs_assault 
by CryptR 
lmuur@dlc.fi

cs_tire
by Davej (Curtains)
dave@3dgaming.com

"Defusion" C4 Bombing Maps:

de_dust
by Davej (Curtains)
dave@3dgaming.com

de_prodigy
by Hobbit
hobbit@bellatlantic.net

de_nuke
by MEEEEDIC
jogi@netads.de


Texture Artists : 
-----------------

Ido Magal
ido@dnai.com 

Chris Ashton
chrisa@presto.com 



____________________________________________________________________



BETA 3.1
[9.16.99]
- Bullet penetration bug fixed
- Radio .wav's now have lower volume
- Removed automatic .wav's (death, flashbang)
- fixed MRAD_ENEMYSPOTTED error
- Disorientation system changed
- Added "ignoreradio" command to only ignore .wav's
- Flashbang Shrapnel altered



BETA 3.0
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

- added new vesion of cs_assault (compatible w/ hlserver.exe)
- added scientist model for hlserver.exe
- added assault's proper sky
- fixed telefragging  (cs_alley will no longer telefrag)
- fixed dropweapon
- fixed those spurious 'player joined' messages
- changed Ak-47 price


BETA 2.0

NEW Features :
- Three new guns added : {Sig SG-552 Commando , AK-47 , Desert Eagle}
- Added silencers to the USP .45 Tactical and the Colt M4A1
- Added a round timer which shows how much time is left in the round
- Added team scores which shows how many rounds a team has won
- Added Night Vision Goggles
- Added new entity for mappers to use (info_hostage_rescue)
- Optimized all the models for lower r_speeds!
- Ability to assign keys to all of the commands from the controls menu  (courtesy of cannelbrae of Gunman project)


-------------------------------------------------------------------



Counter-Stike is a modification (MOD) to the excellent game, Half-Life. It modifies the multiplayer aspects of Half-Life to bring to it a more team-oriented gameplay. Not terribly unlike Team Fortress2, Counter-Strike provides the player with an experience that a trained counter-terrorist unit or terrorist unit experiences. 

The MOD is team-based featuring one team playing the role of the terrorist and the other team playing the role of the anti-terrorist. Each side has access to different guns and equipment, as well as different abilities. Maps will have different goals such as: hostage rescue, assasination, kill the entire opposing force, etc. 

Weapons include the usual assortment of pistols, shotguns, assault rifles, sniper rifles, grenades, demolition devices. Each side has access to a different subset of weapons so it may be the case that only the counter-terrorist can use the M4A1, and only the terrorists can use the AK-47.

We are confident that we've created a MOD quite unlike any other, that is still fun to play and free damnit! 







===============COMMANDS===================



plant_c4
plants the c4 bomb, if the player has one

+showfrags        
displays every player's frag counts on the scoreboard

-showfrags
only displays the player's frag count on the scoreboard

radio1  
The primary set of radio commands to issue to your team.

radio2  
The secondary set of radio commands to issue to your team.

 buyweapon 
Brings up the weapon purchase menu. Weapon purchasing can only be done from near your starting point. 

buyammo 
Brings up the ammo purchase menu. Ammo can only be purchased near your starting point. 

buyitem 
Brings up the item purchase menu. Items can only be purchased near your starting point. 

hostage 
Credits team with a hostage rescue. This is for Counter-Terrorists only. Hostages may only be "rescued" near the Counter-Terrorists starting point. 

showplayerinfo 
Brings up some player stats, including money, player team, and kick voting. 
throwweapon If you happen to own any guns from a purchase, this command will throw it on the ground for later retrieval, or to give to another player. 

ignoremessages 
this command will toggle between the 4 different modes of ignore messages {ignore broadcast messages , ignore team messages + broadcast messages , accept ALL messages} 

nightvision 
Toggles Night Vision Goggles on/off. You must have purchased Night Vision Goggles for this command to work. 

listplayers
Lists all players in a game and assigns them a number for kicking purposes

vote x
Type this with the number of the player in place of x, who you want to kick


**Important! Make sure all number keys are bound properly (ie. bind 7 slot7, bind 8 slot8, etc)




________________________________________________________________________________________________



****** How to use the radio *******

You must bind a key to the command "radio1" and "radio2"
For example, if you wanted the key x to be your radio menu, you 
would type "bind x radio1" at the console with no quotes. 
This command will bring up a list of radio commands that you 
can issue. Repeat this for "radio2" 

If you do not want to hear radio
messages, bind a key to ""ignoremessages". This will toggle 4 
different modes, ignore BOADCAST, ignore BROADCAST/TEAM, 
ignore BROADCAST/TEAM/RADIO, accept ALL
*see full list of binds below





SERVER side variables (These are used by the servers only)

'mp_limitteams'		: This would be used for clan matches, allowing clans to setup the teams without any restrictions.
'mp_lowlag'			: This will not restrict the amount of bullet sparks being spawned.. I suggest you keep it at 1 for cable modem servers
mp_roundtime X    {X is the number of minutes the round lasts. Valid values range between 3 and 9. Default is 5}
 mp_c4timer X      {X is the number of seconds the C4 bomb is set to blow. Valid values range between 10 and 90. Defaults is 30}
 mp_limitteams 0/1 {1 will restrict the number of players per team. Default is 1}
 mp_lowlag 0/1     {0 will causes more bullet sparks to be spawned, thereby creating more lag. Default is 1}
 mp_friendly_grenade_damage 0/1   {1 will result in HE grenades hurting teammates. Default is 1}






How.to.play 
For full information on how to play, visit:
http://www.counter-strike.net/howto.html
courtesy of Tony "Rooster" Orr
adapted by Cliffe




Don't forget to visit the other sites on the Counter-strike.net network!

CSSkins
http://skins.counter-strike.net/

Anarchy Design
http://anarchy.counter-strike.net/

CSNation
http://csnation.counter-strike.net/

CSClanworld
http://clanworld.counter-strike.net/



_____________________________________________________



CREDITS:
--------



The CS Team:

| Name | Gooseman (aka Minh Le)
| E-mail| gooseman@counter-strike.net 
| Position | Project leader, Head modeler, Head coder, Head-job
| Bio | "Rock the kazbah!" 
| Quote | "Unghh.... Damnit J.C."


| Name | CLIFFE (aka William Cleof IV)
| E-mail| cliffe@counter-strike.net 
| Position | Webmaster, 2d-graphics, PR, sound effects, game design etc.
| Bio | enter pretentious bio here 
| Hobbies | I'm a simple man, I enjoy mending things and visiting with the aged.






THANKS: (In no particular order):

Mr_Grim			: for his help in coding the radio system
BETA test team	: for helping us test this shit out.. and for providing the occasional premature leak
Valve Software	: for their constant support
Cliffe			: Radio sounds, and too much to list
Fanny			: for giving me motivation!
Mappers, Texture artists


And special thanks to: Special thanks to the following people: monsieurevil; Oddjob, Mr. Grim, and Dallas Frank of the A-Team; Mindvision for the great installer; Justin; Howie Dorough; Beefy Raunchholes; Yash Chavda; MTG; A.J. McLean; Tony Clifton; shirow @ mod central; Peter North; bosch; A.J. McLean; Eyeburn; all the server admins who have helped us test .dll's; Darkman for the fantastic servers; Rooster @ mod central; rze; Gamefan Network; Adrian @ Gameplay.com; all the CS mappers and texture artists; Cow; Ash; and last but of course not least A.J. McLean. 

The CS Team would also like to thank all the CS players. Without you, the mod is nothing.



Anyone else who we might have missed!

--Readme.txt by Gooseman & Cliffe


