# Player Identification in commands

Commands that accept player names can use different types of input.

## Partial Name

The simplest player identifier is the player name. You can use any part of the player's name. Only enough characters are required to match the player name uniquely. If more than one player on the server has a similar name, you will be prompted with all players matching that name and their client ID.

!!! example
    `!warn jo spec` for giving a warning to a connected player named 'John' for being spec on full server.

!!! note
    You can use the `!find` command to show which connected players match a given name.

## Client ID

The client ID is the number assigned to the player by the game server. The client ID only works for the current game session. Use the command `!list` to display a list of the client IDs of the players. If a player name is too difficult to enter, or there are more than one player with similar names, you can pick them out using the client ID.

!!! example
    `!kick 4 tk` to kick a player connected on game slot number 4.

## Database ID

The database ID is the unique identification of the player within the database. It is prefixed with an ”@” character. This ID is displayed with the `!leveltest` and `!lookup` command. With this ID you can take actions against a player even if that player is not connected.

!!! example
    `!makereg @121` to add the player with the ID @121 to the regular group.

!!! example
    `!tempban @1337 tk 150m` to temporary ban the player with ID @1337 for 2,5 hours for team killing.

!!! note
    You can use the `!lookup` command to find offline players in the database and get their database ID.
