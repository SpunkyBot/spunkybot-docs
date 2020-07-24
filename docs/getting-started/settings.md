# Bot Settings

This document describes the parameters and options of the `settings.conf` file.

## server
- `server_ip`
    - IP address of game server. Default: 127.0.0.1
- `server_port`
    - Port of game server. Default: 27960
- `rcon_password`
    - Password for RCON
- `log_file`
    - Full path of the 'games.log' file, e.g. /opt/urbanterror/.q3a/q3ut4/games.log

## rules

- `show_rules`
    - Enable (1) or disable (0) displaying rules / rotation messages
- `rules_frequency`
    - Interval in seconds between each rule / rotation message. Default: 90
- `display`
    - Display rules as 'chat', 'bigtext' or 'server' message. Options: chat/bigtext/server. Default: chat

## bot
- `ban_duration`
    - Ban duration in days for the command "!ban <name>". Default: 7
- `warn_expiration`
    - Expiration time of warnings in seconds. Set to 0 to disable this feature. Default 240
- `task_frequency`
    - Interval in seconds for checking ping, warnings + spectators. Set to 0 to disable this feature. Default: 60
- `max_ping`
    - Maximum allowed ping, player with higher ping will be kicked. Set to 0 to disable this feature. Default: 200
- `kick_spec_full_server`
    - Warn / kick spectator when more than X players are connected. Set to 0 to disable this feature. Default: 10
- `teamkill_autokick`
    - Enable (1) or disable (0) autokick for team killing. Regulars or higher levels will not get kicked. Default: 1
- `allow_teamkill_bots`
    - Enable (1) or disable (0) team kills of bots without getting kicked. Default 0
- `noob_autokick`
    - Enable (1) or disable (0) autokick of players with low score. Regulars or higher levels will not get kicked. Default: 0
- `spawnkill_autokick`
    - Enable (1) or disable (0) autokick for spawn killing. Admins or higher levels will not get kicked. Default: 0
- `instant_kill_spawnkiller`
    - Enable (1) or disable (0) instant kill for player doing spawn kill. Admins or higher levels will not get killed. Default: 0
- `spawnkill_warn_time`
    - Spawnkill timer in seconds between player respawn and death to issue a warning. Recommended value: 2-5. Default: 3
- `bad_words_autokick`
    - Enable (1) or disable (0) autokick for using bad words. Admins or higher levels will not get kicked. Default: 0
- `show_country_on_connect`
    - Enable (1) or disable (0) displaying message "Player connected from...". Default: 1
- `show_first_kill`
    - Enable (1) or disable (0) displaying message "firstblood" / "first nade kill". Default: 1
- `show_hit_stats_respawn`
    - Enable (1) or disable (0) displaying hit statistics during respawn. Default: 1
- `show_multi_kill`
    - Enable (1) or disable (0) displaying multi-kill and monster-kill messages. Default: 1
- `autobalancer`
    - Enable (1) or disable (0) autobalancing of teams at the end of the round/match. Default: 0
- `allow_teams_round_end`
    - Enable (1) or disable (0) allowing command !teams only at end of the round/match. Default: 0
- `limit_nextmap_votes`
    - Enable (1) or disable (0) limiting successful nextmap votes. Default: 0
- `vote_delay`
    - Interval in seconds for delaying votes after failed vote. Set to 0 to disable this feature. Default: 0
- `kill_survived_opponents`
    - Enable (1) or disable (0) killing of survived opponents when bomb has been exploded/defused. Default: 0
- `spam_bomb_planted`
    - Enable (1) or disable (0) spamming the message "Bomb has been planted" in global chat. Default: 0
- `spam_knife_kills`
    - Enable (1) or disable (0) displaying player's knife kill series as bigtext. Default: 0
- `spam_nade_kills`
    - Enable (1) or disable (0) displaying player's HE grenade kill series as bigtext. Default: 0
- `spam_headshot_hits`
    - Enable (1) or disable (0) displaying player's headshot hit series as bigtext. Default: 0
- `reset_headshot_hits_mapcycle`
    - Enable (1) or disable (0) option to reset headshot stats for all players at map rotation. Default: 1
- `reset_kill_spree_mapcycle`
    - Enable (1) or disable (0) option to reset kill spree stats for all players at map rotation. Default: 1
- `verbose`
    - Enable (1) or disable (0) debug messages. Default: 0

## mapcycle
- `dynamic_mapcycle`
    - Enable (1) or disable (0) dynamic mapcycle. If enabled, the rotation of small or big_cycle will be used. Default: 0
- `switch_count`
    - When server reaches the number of players, the map rotation will be switched to 'big_cycle' list. Default: 4
- `small_cycle`
    - Comma separated list of valid map names
- `big_cycle`
    - Comma separated list of valid map names

## lowgrav
- `support_lowgravity`
    - Enable (1) or disable (0) support for Low Gravity Server. Default: 0
- `gravity`
    - Set g_gravity to given value. Default: 800
