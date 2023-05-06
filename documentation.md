---
description: APIs Usage
---

# Documentation

Welcome to the documentation for BaimoRconAPI.

This plugin provides several commands for controlling the server, including commands for managing players.

### Player Commands

#### Get Player Position

```
/baimoapi player getPos <player-name>
```

Returns the player's current position in block coordinates.

#### Get Player UUID

```
/baimoapi player getUuid <player-name>
```

Returns the UUID of the specified player.

#### Get Player World

```
/baimoapi player getWorld <player-name>
```

Returns the name of the world that the specified player is currently in.

#### Get Player Health

```
/baimoapi player getHealth <player-name>
```

Returns the current health value of the specified player.

#### Get Player Hunger

```
/baimoapi player getHunger <player-name>
```

Returns the current hunger value of the specified player.

#### Get Player Experience

```
/baimoapi player getExp <player-name>
```

Returns the current experience value of the specified player.

#### Get Player Experience Level

```
/baimoapi player getExpLevel <player-name>
```

Returns the current experience level of the specified player.

#### Get Player Allow Flight

```
/baimoapi player getAllowFlight <player-name>
```

Returns whether or not the specified player is currently allowed to fly.

#### Get Player Speed

```
/baimoapi player getSpeed <player-name> [walk | fly]
```

Returns the current speed (either walking or flying, depending on the mode specified) of the specified player.

#### Set Player Display Name

```
/baimoapi player setDisplayName <player-name> <new-display-name>
```

Sets the display name of the specified player.

#### Set Player Compass Target

```
/baimoapi player setCompassTarget <player-name> <x> <y> <z>
```

Sets the target location for the specified player's compass.

#### Get Player Locale

```
/baimoapi player getLocale <player-name>
```

Returns the locale of the specified player.

#### Get Player Client View Distance

```
/baimoapi player getClientViewDistance <player-name>
```

Returns the client view distance of the specified player.

#### Get Player Bed Spawn Location

```
/baimoapi player getBedSpawnLocation <player-name>
```

Returns the location of the bed where the specified player will respawn, or "none" if they have not set a bed spawn location.
