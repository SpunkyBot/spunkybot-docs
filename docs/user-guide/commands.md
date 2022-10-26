# Bot Commands

Also check the full list of [commands](https://spunkybot.de/docs/commands) with shortcut commands and required parameters.

```
!command <required parameters> [<optional parameters>] - description
```

## Guest

* `!bombstats` - display Bomb stats
* `!ctfstats` - display Capture the Flag stats
* `!forgive [<name>]` - forgive a player for team killing
* `!forgiveall` - forgive all team kills
* `!forgivelist` - list all players who killed you
* `!forgiveprev` - forgive last team kill
* `!freezestats` - display freeze/thawout stats
* `!grudge [<name>]` - grudge a player for team killing, a grudged player will not be forgiven
* `!help` - display all available commands
* `!hestats` - display HE grenade kill stats
* `!hits` - display hit stats
* `!hs` - display headshot counter
* `!knife` - display knife kill stats
* `!register` - register yourself as a basic user
* `!spree` - display current kill streak
* `!stats` - display current map stats
* `!teams` - balance teams
* `!time` - display the current server time

----

## User

* `!regtest` - display current user status
* `!xlrstats [<name>]` - display full player statistics
* `!xlrtopstats` - display the top players

----

## Moderator

* `!admintest` - display current admin status
* `!country <name>` - get the country of a player
* `!lastmaps` - list the last played maps
* `!lastvote` - display information about the last called vote
* `!leveltest [<name>]` - get the admin level for a given player or myself
* `!list` - list all connected players
* `!locate <name>` - display geolocation info of a player
* `!mute <name> [<duration>]` - mute or un-mute a player
* `!nextmap` - display the next map in rotation
* `!poke <name>` - notify a player that he needs to move
* `!seen <name>` - display when a player was last seen
* `!shuffleteams` - shuffle the teams
* `!spec` - move yourself to spectator
* `!startdemo <name>` - start recording of serverside demo
* `!stopdemo <name>` - stop recording of serverside demo
* `!warn <name> [<reason>]` - warn player
* `!warninfo <name>` - display how many warnings a player has
* `!warnremove <name>` - remove a player's last warning
* `!warns` - list the warnings
* `!warntest <warning>` - test a warning

----

## Admin

* `!admins` - list all the online admins
* `!afk <name>` - force a player to spec, because he is away from keyboard
* `!aliases <name>` - list the aliases of a player
* `!bigtext <text>` - display big message on screen
* `!exit` - display last disconnected player
* `!find <name>` - display the slot number of a player
* `!force <name> <blue/red/spec> [<lock>]` - force a player to the given team
* `!kick <name> <reason>` - kick a player
* `!nuke <name>` - nuke a player
* `!regulars` - display the regular players online
* `!say <text>` - say a message to all players
* `!tell <name> <text>` - tell a message to a specific player
* `!tempban <name> <duration> [<reason>]` - ban a player temporary for the given period of 1 sec to 3 days
* `!warnclear <name>` - clear the player warnings

----

## Full Admin

* `!ban <name> <reason>` - ban a player for several days
* `!baninfo <name>` - display active bans of a player
* `!ci <name>` - kick player with connection interrupt
* `!forgiveclear [<name>]` - clear a player's team kills
* `!forgiveinfo <name>` - display a player's team kills
* `!id <name>` - show the IP, guid and authname of a player
* `!kickbots` - kick all bots
* `!ping <name>` - display the ping of a player
* `!rain <on/off>` - enables or disables rain
* `!scream <text>` - scream a message in different colors to all players
* `!slap <name> [<amount>]` - slap a player (a number of times)
* `!status` - report the status of the bot
* `!swap <name1> [<name2>]` - swap teams for player A and B
* `!version` - display the version of the bot
* `!veto` - stop voting process

----

## Senior Admin

* `!addbots` - add up to 4 bots to the game
* `!banall <pattern> [<reason>]` - ban all players matching pattern
* `!banlist` - display the last active 10 bans
* `!bots <on/off>` - enables or disables bot support
* `!clear` - clear all player warnings
* `!cyclemap` - cycle to the next map
* `!exec <filename>` - execute given config file
* `!gear <default/all/knife/pistol/shotgun/sniper/magnum/mac>` - set allowed weapons
* `!instagib <on/off>` - set Instagib mode
* `!kickall <pattern> [<reason>]` - kick all players matching pattern
* `!kill <name>` - kill a player
* `!lastadmin` - display the last disconnected admin
* `!lastbans` - list the last 4 bans
* `!lookup <name>` - search for a player in the database
* `!makereg <name>` - make a player a regular (Level 2) user
* `!map <ut4_name>` - load given map
* `!mapcycle` - list the map rotation
* `!maprestart` - restart the map
* `!maps` - display all available maps
* `!moon <on/off>` - activate low gravity mode (Moon mode)
* `!permban <name> <reason>` - ban a player permanent
* `!putgroup <name> <group>` - add a client to a group
* `!rebuild` - sync up all available maps
* `!setgravity <value>` - set the gravity (default: 800)
* `!setnextmap <ut4_name>` - set the next map
* `!swapteams` - swap the current teams
* `!unban <@ID>` - unban a player from the database
* `!unreg <name>` - remove a player from the regular group

----

## Super Admin

* `!bomb` - change gametype to Bomb
* `!ctf` - change gametype to Capture the Flag
* `!ffa` - change gametype to Free For All
* `!gametype <bomb/ctf/ffa/tdm/ts>` - set game type
* `!gungame` - change gametype to Gun Game
* `!jump` - change gametype to Jump
* `!lms` - change gametype to Last Man Standing
* `!password [<password>]` - set private server password
* `!reload` - reload map
* `!tdm` - change gametype to Team Deathmatch
* `!ts` - change gametype to Team Survivor
* `!ungroup <name>` - remove admin level from a player

----

## Head Admin

* `!putgroup <name> <group>` - add a client to a group (Moderator to Super Admin)
