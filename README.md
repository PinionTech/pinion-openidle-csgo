# OpenIdle: Counter-Strike: Global Offensive

OpenIdle is a free/public SourceMod plugin designed to provide a number of features to your idle server.   This version is for CS:GO, but it may be ported to other games in the future.


## Features

* Force players to join a team on connect.
* Respawn players automatically on death (delay configurable).
* Deal damage to idle players, with options for delay, damage, and frequency.
* Create custom spawn locations per map.
* Supports [Updater](https://forums.alliedmods.net/showthread.php?t=169095).

## Install

1. Copy the plugin into your plugins directory.
2. Copy the configs into /cfg/sourcemod/

See the folder structure in the repo for details.

## Commands

* **sm_setspawn <T / CT>**:   Create a new spawn location for team T or CT at your current location.  Requires ADMFLAG_ROOT command access.

## CVARs
*Change these options in /cfg/sourcemod/openidle.cfg*

| Cvar & Default Value | Effect |
|--|--|
| **sm_openidle_customspawns_enabled "1"** | // Set to 0 to disable custom spawns.  Spawns must be placed per map using sm_setspawn. |
|**sm_openidle_forceteam "1"** |// Set to 0 to disable forcing players to teams.|
| **sm_openidle_idledamage_amount "10"** |// The amount of damage to apply to idle players for each time they are found idle.|
| **sm_openidle_idledamage_enable "1"** |// Set to 0 to disable dealing damage to idle players.|
| **sm_openidle_idledamage_frequency "1"** |// The number of seconds to wait before damaging an idle player again.
|**sm_openidle_idledamage_idletime "30"**|// The number of seconds a player must be stationary to be counted as idle.|
|**sm_openidle_respawn_enabled "1"**|// set to 0 to disable automatic respawn.|
|**sm_openidle_respawndelay "5.0"**|// The number of seconds to wait before respawning a player.|
|**sm_openidle_runconfig "1"**|// Run sourcemod/openidle.serverconfig.cfg at the start of rounds?|


## About

* Plugin developed by [Caelan Borowiec](https://gitlab.com/CaelanBorowiec/).
* Development sponsored by [Pinion.gg](https://www.pinion.gg/).
