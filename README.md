# Counter-Strike Beta 4.0

## Supported versions
- [x] **Windows**
- [x] **Linux**

## Recommended Half-Life / HLDS version to play
- Windows: Half-Life v1.0.1.6 
- Linux: Half-Life Dedicated Server v3.0.1.6

_____

# Changelog

```
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
```