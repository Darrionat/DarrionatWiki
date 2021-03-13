---
description: Detailed Information on all commands and their permissions
---

# Commands & Permissions

Command information can also be seen with **/prisonpick help** or with the [Help GUI]().  
If a player does not send enough arguments for the subcommand that they used, they will be sent the help message for that command.   
Commands that directly affect a player using the command cannot be run by the console.

### Commands

| Command | Function | Console Can Use |
| :--- | :--- | :--- |
| /prisonpick | Shows base message | true |
| /prisonpick bypass | Allows a player to be able to move a pickaxe in their inventory | **false** |
| /prisonpick help | More command information | true |
| /prisonpick helpGui | Opens a GUI that contains more command information | **false** |
| /prisonpick reload | Reloads all config files and settings | true |
| /prisonpick removePickaxe \[player\] | Removes a pickaxe from a specified player | true |
| /prisonpick resetPlayer \[player\] | Resets all of a player's enchantments and their blocks mined to 0 | true |
| /prisonpick setEnchant \[player\] \[enchant\] \[level\] | Sets a player's level for a specific enchantment | true |

### Permissions

All permissions are based on the format of **prisonpick.subCommand**. So for example, a valid permission would be **prisonpick.setenchant**.   
Without permission for a specific command, a player will not be able to use that command. Opped players will have permission for all commands. 

