# VIPRespawns [![Build Status](https://travis-ci.org/condolent/VIPRespawns.svg?branch=master)](https://travis-ci.org/condolent/VIPRespawns) [![Chat on Gitter](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/VIPRespawns/Lobby) [![Releases](https://img.shields.io/badge/release-1.5.8-orange.svg)](https://github.com/condolent/VIPRespawns/releases) ![Branch](https://img.shields.io/badge/branch-master-lightgrey.svg)
Sourcemod plugin. Allowing players with A-flag respawn x times per map!  
[AlliedMods](https://forums.alliedmods.net/showthread.php?p=2523408#post2523408)

## Usage
Players with the `a`-flag gets 3 respawns per map.  
To respawn, you simply use the command `!vipspawn` when dead.  
You can also check how many respawns you have left via `!spawnsleft`.  
A menu available via `!vip`, as long as it has not been disabled in config.

## Downloads
[Releases](https://github.com/condolent/VIPRespawns/releases)  
[Website](https://condolent.xyz/VIPRespawns/)

## Installation
Simply download the `viprespawn.smx` file via the link above and drag the file to `/addons/sourcemod/plugins`.

Then execute command in server console:  
`sm plugins load viprespawn`

To mod the plugin you will need the [colors](https://forums.alliedmods.net/showthread.php?t=96831) include.

## Configuration
The config-file is located in `root/csgo/cfg/sourcemod/viprespawns.cfg`. In there you can change some options.

This is how the config looks like:
```
// This file was auto-generated by SourceMod (v1.8.0.5998)
// ConVars for plugin "viprespawn.smx"

// Enable the VIP-menu called with !vip?
// (0 = Disable, 1 = Enable)
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
sm_enable_vip_menu "1"

// Amount of times a user is allowed to respawn per map
// -
// Default: "3"
sm_respawn_amount "3"

// How many players needs to be alive in order to respawn
// Set 0 to allow all the time.
// - 
// Default: "3"
sm_minimum_players_alive "3"

// Should the sm_minimum_players_alive only count players playing on a specific side?
// 0 = Disable. 1 = Track terrorists. 2 = Track counter-terrorists.
// -
// Default: "0"
sm_minimum_players_alive_side "0"
```

## Translation
Want to help translate the plugin?  
Create a [Pull request](https://github.com/condolent/VIPRespawns/pulls) and edit the viprespawn.phrases.txt with your language added. Or you can create a [ticket](https://github.com/condolent/VIPRespawns/issues) with and write which language you're fluent within!



### Credits
Props to [B2SX](https://forums.alliedmods.net/member.php?u=265974) for creating the base-code for respawns!  
What I did was clean the code a bit and added some more end-user friendly properties.
