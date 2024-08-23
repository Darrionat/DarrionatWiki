---
description: A GUI is a menu that can be opened by a player
---

# GUIs

Being available to players, the GUIs in PrisonPick serve a similar purpose: to make it easy for the player to perform an action or fetch information. The [Help GUI](guis.md#help-gui) and the [Pickaxe GUI](guis.md#pickaxe-gui) both do this. Items may not be removed from the GUI and the player will be prevented from clicking any items in their inventory as well.

## Help GUI

The Help GUI is a GUI that can be opened when a player uses the command `/prisonpick helpgui`. The player will be presented with a menu of base commands which, if applicable, can be clicked to view their subcommands.\
The fill material for both the Base Command GUI and the SubCommand GUI is black stained glass panes.\
\
The Help GUI is most likely the least customizable aspect of the plugin because it is only available to admins and is automatically changed based upon how many commands there are. This is so that I, the developer, do not have to change a part of the GUI every time I add/remove/change a command in the plugin.

### Base Command GUI

If a command has subcommands it's presented as a CHEST\_MINECART; otherwise, it will be presented as a MINECART. Every base command will be displayed with the item name being the base command and the lore being subcommands. The base command will be displayed with its most basic alias, such as `/prisonpick`.

{% hint style="info" %}
The lore will most likely include a description of the base command when there is a base command added that does not have any subcommands.
{% endhint %}

![A base command within the Base Command GUI](../../.gitbook/assets/javaw\_8teGAB4BNA.png)

### Subcommands GUI

Subcommands are displayed through this GUI. Each subcommand will be displayed as a MINECART because a subcommand cannot have a subcommand. Detailed information about subcommands can be found within the lore of the item. This information is fetched from the [messages.yml](configuration-files/messages.yml-1.0.2.md), so the information of subcommands can be customized to a degree.

![A subcommand within the Subcommand GUI](../../.gitbook/assets/javaw\_mKi71G8iOQ.png)

## Pickaxe GUI

The Pickaxe GUI is opened when a player right-clicks their custom item. This GUI is used to upgrade [enchantments](enchantments.md). The displayed name of the GUI, the number of rows in the GUI, and the fill item \[an item that occupies all empty slots] for the GUI can all be customized within the [config.yml](configuration-files/config.yml-1.0.2.md). Adding an enchantment will update the player's items to whatever new stats they have. Where/how this data is saved is mentioned [here](saving-data.md).\
\
Enchantments can also be upgraded in different amounts based upon the click type. This can be changed in the [enchants.yml](configuration-files/enchants.yml-1.0.2.md). Setting any of these to **MAX** will make it automatically calculate the max amount of levels that it can upgrade with the player's current balance.

| Click Type        | Upgrade Amount |
| ----------------- | -------------- |
| Left-Click        | 1              |
| Right-Click       | 10             |
| Shift Right-Click | 100            |
| Middle-Click      | MAX            |

{% hint style="info" %}
There will most likely be a way to display any item you want in the pickaxe GUI in the future. This will allow for placeholders, stats, etc to be displayed.
{% endhint %}

![The Night Vision enchantment within the Pickaxe GUI](../../.gitbook/assets/javaw\_0HU4taahUT.png)
