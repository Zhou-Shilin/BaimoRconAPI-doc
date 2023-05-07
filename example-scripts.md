# Example Scripts

```python
import pyrcon
import time
import subprocess

# Connect to the Minecraft server using rcon
rcon = pyrcon.PyRCON('localhost', 25575, 'rconpassword')
rcon.connect()

while True:
    # Get the player list using "/list" command
    player_list = rcon.command('list')
    player_names_list = player_list.split(':')[1].split(', ')
    for player_name in player_names_list:
        # Get the health of each player using BaimoRconAPI
        health_response = rcon.command(f'/baimoapi player getHealth {player_name}')
        # Parse the health value from the response
        health_value = float(health_response.split('=')[1])

        if health_value < 2:
            # Set the player's display name to "[Dying] Origin Player Name" using BaimoRconAPI
            display_name = f'[Dying] {player_name}'
            set_display_name_response = rcon.command(f'/baimoapi player setDisplayName {player_name} {display_name}')
            # Print the response to the console
            print(set_display_name_response)

    # Wait for 5 seconds before running the command again
    time.sleep(5)

rcon.disconnect()

```

This example connects to a Minecraft server using rcon and continuously checks the health of all players in the player list. If a player's health is less than 2, the script sets their display name to "\[Dying] Origin Player Name" using BaimoRconAPI. The responses from BaimoRconAPI commands are printed to the console. The script waits for 5 seconds before checking the player list again to avoid flooding the server with requests.This example connects to a Minecraft server using rcon and continuously checks the health of all players in the player list. If a player's health is less than 2, the script sets their display name to "\[Dying] Origin Player Name" using BaimoRconAPI. The responses from BaimoRconAPI commands are printed to the console. The script waits for 5 seconds before checking the player list again to avoid flooding the server with requests.
