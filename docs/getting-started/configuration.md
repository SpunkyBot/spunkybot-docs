# Configuration

This document describes the configuration of your game server that is required in order to work properly with Spunky Bot.

## Urban Terror Game Server

Make sure your game server config sets the following CVAR parameters correctly:

```
seta g_logsync      "1"  // real-time log writing
seta g_loghits      "1"  // log all hits (allows to recognize headshots)
seta g_friendlyfire "2"  // friendlyfire enabled but no kicks
```

Otherwise open your server config file, e.g. `sudo vi /opt/urbanterror/.q3a/q3ut4/server.cfg` and modify these parameters.

!!! note "Note"
    Restart your Urban Terror game server to apply the changes.

## Spunky Bot Settings

Open the configuration file `/conf/settings.conf` in your Spunky Bot folder and change at least the IP address, port, RCON password and the full path of the `games.log` log file according to your environment.

Detailed configuration options of Spunky Bot can be found in the [settings](settings.md) guide.

!!! note "Note"
    Restart Spunky Bot to apply the changes.

## Running Spunky Bot

You can run Spunky Bot from the command line:

```bash
$ python spunky.py
```

Or use the provided initscript as described [here](#advanced-configuration).

## First start instruction

After successfully installing and configuring Spunky Bot, you will start the bot for the first time.
Spunky Bot will check if there is a **Head Admin** in your database. If not, the command `!iamgod` will be enabled for the first player typing it in the game.

Connect to your game server and type `!iamgod` in the global chat to get the admin level **Head Admin**.
This command will be disabled automatically. Spunky Bot allows only one user as Head Admin.

## Advanced Configuration

Use the provided systemd script to run Spunky Bot as daemon:

* Modify 'User' and 'WorkingDirectory' to suit where you installed Spunky Bot
* Move this file to /lib/systemd/system/spunkybot.service
* Reload systemctl daemon: `sudo systemctl daemon-reload`
* Start the Bot at server boot: `sudo systemctl enable spunkybot.service`
* Manual start of the Bot: `sudo systemctl start spunkybot.service`

Use the provided sysVinit script to run Spunky Bot as daemon:

* Modify the lines 20-25 of the file debian_startscript to suit where you installed Spunky Bot, and which user is running the Urban Terror server
* Move the file to /etc/init.d/spunkybot: `sudo mv debian_startscript /etc/init.d/spunkybot`
* Make it executable: `sudo chmod +x /etc/init.d/spunkybot`
* Start the Bot at server boot: `sudo update-rc.d spunkybot defaults`
* Manual start of the Bot: `sudo /etc/init.d/spunkybot start`
