---
description: List of commands and permissions
---

# Commands & Permissions

### Base Command - /cc

Permission: commandcooldown.use

| **Command**                   | **Description**                                | Permission                          |
| ----------------------------- | ---------------------------------------------- | ----------------------------------- |
| /cc help \[page]              | Shows a help list                              | commandcooldown.help                |
| /cc list                      | Shows a list of all cooldowns                  | commandcooldown.list                |
| /cc bypass                    | Bypasses all cooldowns                         | commandcooldown.bypass              |
| /cc reload                    | Reloads the config.yml                         | commandcooldown.reload              |
| /cc editor                    | Enter the command cooldown GUI editor          | commandcooldown.editor              |
| /cc removecooldowns \[player] | Removes all current cooldowns from a player    | commandcooldowns.removecooldowns    |
| /cc cooldowns                 | Prints out the player's current  cooldows      | commandcooldown.cooldowns (default) |
| /cc cooldowns \[UUID/player]  | Prints the current cooldowns of a given player | commandcooldown.cooldowns.others    |



### Other Permissions

| Permission                               | Description                                                                                                                                          |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| commandcooldown.bypass.command\_here     | Bypass a certain command with permission. Spaces are replaced with underscores                                                                       |
| commandcooldown.**command**.**cooldown** | <p>Example: commandcooldown.home.30</p><p>This would change the cooldown to 30 seconds for a player/group instead of the default for the command</p> |
