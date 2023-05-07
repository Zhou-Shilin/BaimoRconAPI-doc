---
description: APIs Usage
---

# Documentation

BaimoRconAPI is a Bukkit plugin that allows Rcon clients to execute server commands and retrieve player and block information using a set of API commands.

### Commands

#### `/baimoapi player getPos <playerName>`

Description: Retrieve a player's current coordinates.

Example Return: `x=0, y=64, z=0`

#### `/baimoapi player getUuid <playerName>`

Description: Retrieve a player's unique identifier.

Example Return: `UUID=uuid-here`

#### `/baimoapi player getWorld <playerName>`

Description: Retrieve the world a player is currently in.

Example Return: `World=world_name`

#### `/baimoapi player getHealth <playerName>`

Description: Retrieve a player's health value.

Example Return: `Blood=20.0`

#### `/baimoapi player getHunger <playerName>`

Description: Retrieve a player's hunger value.

Example Return: `Hunger=20`

#### `/baimoapi player getExp <playerName>`

Description: Retrieve a player's current experience value.

Example Return: `Experience=0.5`

#### `/baimoapi player getExpLevel <playerName>`

Description: Retrieve a player's current experience level.

Example Return: `Experience Level=1`

#### `/baimoapi player getAllowFlight <playerName>`

Description: Retrieve whether a player is allowed to fly or not.

Example Return: `Allow Flight=true`

#### `/baimoapi player getSpeed <playerName> <walk/fly>`

Description: Retrieve a player's walking or flying speed.

Example Return: `Walk Speed=0.2`

#### `/baimoapi player setDisplayName <playerName> <displayName>`

Description: Set a player's display name.

Example Return: `msg=Success`

#### `/baimoapi player setCompassTarget <playerName> <x> <y> <z>`

Description: Set a player's compass target.

Example Return: `msg=Success`

#### `/baimoapi player getLocale <playerName>`

Description: Retrieve a player's current locale.

Example Return: `Locale=en_us`

#### `/baimoapi player getClientViewDistance <playerName>`

Description: Retrieve a player's client view distance.

Example Return: `Client View Distance=10`

#### `/baimoapi player getBedSpawnLocation <playerName>`

Description: Retrieve a player's current bed spawn location.

Example Return: `Bed Spawn Location=world_name, 0, 64, 0`

#### `/baimoapi block getID <x> <y> <z>`

Description: Retrieve the ID of a block at a certain location.

Example Return: `BlockID=dirt`

#### `/baimoapi block getFace <x> <y> <z>`

Description: Retrieve the face of a block at a certain location.

Example Return: `BlockFace=north`

#### `/baimoapi block searchForBlock <x1> <y1> <z1> <x2> <y2> <z2> <blockId>`

Description: Search for a specific type of block within a defined area.

Example Return: `Block={x=0, y=64, z=0}`
