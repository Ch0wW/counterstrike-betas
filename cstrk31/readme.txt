
Counter-Strike Mod for Half-Life
http://www.counter-strike.net/
Readme.txt
______________________________________


BETA 3.1
[9.16.99]
- Bullet penetration bug fixed
- Radio .wav's now have lower volume
- Removed automatic .wav's (death, flashbang)
- fixed MRAD_ENEMYSPOTTED error
- Disorientation system changed
- Added "ignoreradio" command to only ignore .wav's








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
- siege, bunker, desert updated
- added cs_tire.bsp
- added cs_militia.bsp
- added cs_hideout.bsp
- added cs_ship.bsp
- re-added cs_mansion.bsp to map rotation


****** How to use the radio *******

You must bind a key to the command "radio" For example, if you wanted
the key x to be your radio menu, you would type
"bind x radio" at the console with no quotes. This command will
bring up a list of radio commands that you can issue. A "commander"
is randomly selected every round. You should also bind a key to 
the command "commanderradio" Use this key when you are selected
as the commander for that round. This will enable you to issue
special commander only commands such as "Get in position..."
and "Follow my lead" etc. If you do not want to hear radio
messages, bind a key to ""ignoremessages". This will toggle 4 
different modes, ignore BOADCAST, ignore BROADCAST/TEAM, 
ignore BROADCAST/TEAM/RADIO, accept ALL
*see full list of binds below


******* General tips for BETA 3.0 ********
- The commander of each team is chosen at random at the beginning of a round.
The commander is not only capable of sending regular radio messages, but also
special commander radio messages ("commanderradio"). These special commander
messages can greatly help co-ordinate an attack. Use them wisely!
- The effective range of the submachine guns and the assault rifles must be 
paid attention to. On large maps such as CS_SIEGE , a rifle is a much better
weapon since it's damage at longer ranges doesn't diminish as quickly as a
sub-machine gun or a pistol. On smaller maps with tight in fighting, a SMG's
accuracy or a shotgun's spread will be a valuable asset. Learn to pick the
right weapon for the right situation!
- The helmet is a real life saver and will make a distinctive noise when hit.
The POV will be skewered so severely that returning fire would be a moot
point.. It's best to find cover quickly and count your lucky stars you're alive
Some of the high powered guns will defeat the helmet at close range with one
shot.




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



------------------------------------------------------------------------------------------------------------------------
=======COMMANDS========



commanderradio
This bind let's the commander only issue special orders

radio  
All players on a team have access to these 9 commands

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




___________________________________________________________________________________________________________________________





SERVER side variables (These are used by the servers only)

'mp_limitteams'		: This would be used for clan matches, allowing clans to setup the teams without any restrictions.
'mp_lowlag'			: This will not restrict the amount of bullet sparks being spawned.. I suggest you keep it at 1 for cable modem servers















How.to.play 
http://www.counter-strike.net/howto.html
courtesy of Tony "Rooster" Orr
adapted by Cliffe

What you need: 
First you'll need a full registered version of Half-Life. Install the latest HL patch. Next go to the Counter-Strike downloads page and grab the latest CS install file[s]. Installation is a breeze. Just locate the files, double-click on them point them towards you Half-Life directory, and let it install. 

The controls: 
The first time you run Counter-Strike, all the controls are set to the default configuration. This means that you will need to go in and set all of your control settings you wish to use in Counter-strike; the controls you set for Half-Life will have no effect within Counter-Strike. Half-Life maintains each mods controls seperate and apart from the regular control set, so you need to make sure you set ALL controls with the mod activated




Show Me The F'n Money: 
Various actions in Counter-Strike will let you gain or lose money. Below is a list of all money matters:

Touching a hostage :
- $150 given immediately to the CT player who first touches the hostage
- $150 added to the CT account (i.e. all CT players will get $150 added to their accounts at the end of the round)
- so in summary, the first CT to touch a hostage will get $300 just for touching him ($150 immediately, and another $150 at the end of the round)

Rescuing a hostage :
- $500 given immediately to the CT player who brings the hostage back to the rescue points
- $350 given to each CT at the end of the round for each hostage rescued.

Hostage Bonus (money awarded to the team that has won a round based on the number of hostages kept alive)
- $400 for each hostage kept alive is given to every player of the team that has won the round
- In short, more money is given for actually rescuing a hostage, than simply leaving him alive. 

Round Win Bonus :
- $500 given to each member of the team that wins a round

Charity Bonus :
- $800 given to each member of the losing team

Killing an enemy :
- $300 given to the player

Killing a teammate :
- $1800 DEDUCTED from the player's account

Killing a hostage :
- $850 DEDUCTED from the player's account

Hitting an enemy :
- $10 given to the player 

The Gameplay: 
There are two teams: one a team of terrorists, and the other a team of counter-terrorists. Sounds good so far, eh? At the start of the map, the terrorists are holed up, usually in a building, with some hostages. Their goal is to keep as many hostages as they can from being rescued, while wiping out as many counter-terrorists as possible. The Counter-terrorists, on the other hand, need to infiltrate the terrorists hidey-hole, rescue as many hostages as possible, and wipe out as many terrorists as they can. The game progresses in a series of matches, with the match ending under one of the following circumstances:

All terrorists killed (counter-terrorists win) 
All counter-terrorists killed (terrorists win) 
6 1/2 minutes expire - (draw) 

 When you start the game off, you will have only your standard issue weapon with a full clip, and another clip of ammo, and that's it. As the game progresses, you are awarded cash for deeds of derring-do. You will use this money to buy yourself new weapons, ammo, and items to make yourself an even more efficient fragging machine. You will also be able to pick up weapons dropped by the dead. It is important to remember that you can only carry one primary weapon (a weapon other than your standard issue) at a time. If, for example, you hold the MP5, and you purchase the m249, you will drop the MP5 on the ground. If, during the course of gameplay, you come across a weapon lying upon the ground from either a fallen comrade, or a fragged enemy, you will need to manually drop your primary weapon by pressing the key you bound to the "dropweapon" command when you set the controls. Please remember not to pick up weapons found lying around your teams spawning area. It is a popular practice to leave weapons lying around as a back-up, and you don't really want to steal your teammates stuff, as it really doesn't endear you to your team to do stuff like that. 

Misc. tips
- When a player joins a server, he is assigned a default team.
- If you put your crosshair over a player for a second, his name will appear onthe screen.
- Teams can be distinguished on the scoreboard by the colour of the players names. Terrorists are written with red text whereas the Counter-terrorists are written with white text.
- Accuracy of the weapons are affected by whether or not the player is ducking/standing/running.
- Flashbang effects are minimized if you turn away from the flashbang before it explodes.
- Kevlar vests are an important tool but bear in mind they don't protect your head.

Buying stuff 
 So you've rescued some hostages, scored some frags, and won a few rounds. You should now have quite a nice stash of cash. When you set you controls, one of the commands you set should have been a "Show Player Info" command. Press this key, and it will breing up a display in the right side of the screen, showing your current balance of cash, you team, and any players you have currently voted to kick out of the game. The most important item here is the cash, though : ) After checking out how much you have, it's time to shop! 

Want to purchase a weapon? Of course you do! Press the key you selected for "Purchase Weapon". A menu will appear onthe right side of the screen with several choices of weapon catagories. Select the number of the catagory you want, and another menu will appear of weapons in that catagory, with prices listed along side. Pick the one you want, or can afford, and it's yours! Now you will want some ammo, as newly purchased weapons only come with a full magazine, and no more. Press the "Purchase Ammo" key, and locate the ammo that is used for your weapon. Make sure you choose the right kind, though! Items are purchased in the same manner. For the scoring screen, RED is terrorists, white is counter-terrorist. 

How the f*** do I join a game?: 
The best way to find Counterstrike servers is with Gamespy. You'll also want to grab the Counter-Strike Gamespy tab. Just download and install, sort by game, and hop on whatever Counterstrike server tickles your fancy. Remember, when you join a game you may not be able to start playing right away and you'll be in spectator mode. Once the round ends, you'll be able to start playing. Have fun! 



**All text and taken from HL Mod Central's Quick and Dirty Guide to Counter-Strike. Take a look at it for more complete info, weapon info, and item info. 



CREDITS (In no particular order):

McClane			: for helping radio-ize
Mr_Grim			: for his help in coding the radio system
BETA test team	: for helping us test this shit out.. and for providing the occasional premature leak
Valve Software	: for their constant support
Cliffe			: too much to list
Viper-X			: HUD graphics and miscellaneous skin jobs
Fanny			: for giving me motivation!
Mappers, Texture artists

Anyone else who we might have missed!
