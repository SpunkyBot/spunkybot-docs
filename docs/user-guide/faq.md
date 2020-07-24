# Frequently Asked Questions

[TOC]

## How do I become Head Admin?

Connect to your game server and be the first to enter `!iamgod` in the global game chat.

## Someone entered !iamgod before me! How to fix this?

Once the `!iamgod` command was used, it is no longer available.

Stop Spunky Bot and delete the database file `data.sqlite`. Then make sure no one is on your game server, restart Spunky Bot and be the first to enter `!iamgod` in the global game chat.

!!! tip
    Use the following sequence of commands to delete the database file:

        $ sudo /etc/init.d/spunkybot stop
        $ sudo rm /opt/spunkybot/data.sqlite
        $ sudo /etc/init.d/spunkybot start

If you do not want to delete your database file, you can remove the user from the _Head Admin_ group by editing the database. To do this, you need a tool to connect to your database.

## Why doesn't Spunky Bot respond to my commands?

If Spunky Bot seems to ignore your commands, follow the instructions to identify the problem:

* restart Spunky Bot
* connect to your game server
* type `!help` in the global game chat

## How do I add administrators?

Use the command `!putgroup` to add a player using the name or ID to one of the admin groups, in this example to the Full Admin group:

```bash
!putgroup <name|id> fulladmin
```

Spunky Bot has several user groups, each serving a specific purpose.

## Spunky Bot responds slow to my commands

If Spunky Bot reads the game server log file, your game log file might not be updated in real-time by the game server.
Check your game server settings according to the instructions in the game configuration section.

## Can I run Spunky Bot on a LAN?

Yes, you can run Spunky Bot on a LAN without limitations.

!!! note
    The "show country on connect" option is deactivated on a LAN.

## Does Spunky Bot run on Windows 64-bit systems?

Spunky Bot runs perfectly on Windows 64-bit operating systems.

## Can I run many different bots?

Yes, you can run many bots on the same machine, as long as you separate them in different folders.

!!! tip "Hint"
    - Bot #1 with home folder: /opt/spunkybot1/
    - Bot #2 with home folder: /opt/spunkybot2/
