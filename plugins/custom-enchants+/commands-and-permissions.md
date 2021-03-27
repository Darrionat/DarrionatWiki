---
description: List of commands and permissions
---

# Commands & Permissions

### Base Command

Permission: customenchants.admin  
Players with this permission will be able to use all commands listed below  
The console will only be able to use  the commands that are marked **true** 'Console Can Use' column

| **Command** | **Description** | Console Can Use |
| :--- | :--- | :--- |
| /ce | Displays the current version | **true** |
| /ce help \[page\] | Returns a page of help messages | true |
| /ce placetable | Places a custom enchantment table - Opens GUI |  |
| /ce removetable | Removes a custom enchantment table |  |
| /ce placeanvil | Places a custom enchantment table - Opens GUI |  |
| /ce removeanvil | Removes a custom enchantment anvil |  |
| /ce placetinkerer | Places a custom enchantment tinkerer - Opens GUI |  |
| /ce removetinkerer | Removes custom tinkerer |  |
| /ce reload | Reloads the config.yml and holograms \(if enabled\) | **true** |
| /ce \[enchant\] \[level\] | Adds a custom enchantment to an item |  |
| /ce list | Displays a list of available enchantments, along with hover text | \*\*\*\* |
| /ce enablegui \[gui\] | Enable a particular gui | **true** |
| /ce disablegui \[gui\] | Disable a particular gui | **true** |
| /ce enableworld \[world\] | Enables the world the player is currently in. \[world\] is optional for players, but required for the console. | **true** |
| /ce disableworld | Disables the world the player is currently in. \[world\] is optional for players, but required for the console. | **true** |
| /ce worldlist | Sends a message for all enabled worlds | **true** |
| /ce updateitems \[player\] | Runs the automatic lore updater through a player's inventory and enderchest. To affect all players, use the "**\***" argument instead of a player name. | **true** |
| /ce givescroll \[player\] \[scroll\] | Gives a certain scroll to a player | **true** |
| /ce giveToken \[enchantment\] \[enchantment Level\] \[player\] | Gives an enchantment token to a player. To affect all players, use the "**\***" argument instead of a player name. | **true** |

### Other Commands

| Command | Description | Permission | Aliases |
| :--- | :--- | :--- | :--- |
| /enchants | Opens up the Enchanter gui | customenchants.enchant | enchantingtable, ench, enchs, enchtable |
| /tinker | Opens up the Tinkerer gui | customenchants.tinker | tink, tinkerer |
| /anvil | Opens up the Anvil gui | customenchants.anvil | anv |

### Other Permissions

| Permission | Description |
| :--- | :--- |
| customenchants.\* | Gives all permissions |
| customenchants.ignoreworlds | Allows a player to ignore disabled worlds |
| customenchants.towny.bypass | Allows a player to bypass CustomEnchants+ Towny protection, if Towny is enabled. |

