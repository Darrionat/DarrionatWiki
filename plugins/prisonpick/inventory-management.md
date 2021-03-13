---
description: How the plugin manages a player's inventory
---

# Inventory Management

PrisonPick is able to manage a player's inventory and their custom item. It has multiple features that allow for a unique experience, and all features listed below can be toggled within the [config.yml](configuration-files/config.yml-1.0.2.md). 

{% hint style="danger" %}
If any player has multiple pickaxes that they are the owner of, they most likely have found a way to duplicate them. Although the [update timer](inventory-management.md#update-timer) will remove illegal items \(if enabled\), please report this and attempt to find out how the player duplicated their custom item.
{% endhint %}

### Breaking Blocks

When the player breaks a block, the plugin can do the following things, if they are enabled:

#### Blocks to Inventory

When a player mines, blocks will be directly put into their inventory. This can be applied to all blocks that are broken by the player. Drops will also be changed according to what level of [Fortune](enchantments.md#fortune) the player is using.  
If the player's inventory is full, by default, drops will be dropped on the ground - this is configurable.

#### EXP to Inventory

When a player mines, any experience that is dropped will directly be given to the player.

### Player Join

#### Give Custom Item

If a player does not have a custom item that they own within their inventory, they will be given a new custom item. Depending on how [data is saved](saving-data.md), their stats may be restored.

#### Update Custom Item

When a player joins, the lore of their pickaxe will be automatically updated to their statistics. If nothing has changed, the lore will be the exact same.

### Prevent Drop

If this option is enabled, it will prevent the player from dropping their custom item.

### Prevent Drop on Death

If enabled, a player's custom item will be dropped when a player dies. This only applies to custom item's that the player is the owner of.

### Prevent Movement

This option will prevent players from moving their pickaxe within their inventory. A player in creative mode or a player using [`/pp bypass`](commands-and-permissions.md#commands) will bypass this prevention. 

### Update Timer

The update timer, if enabled, will \[by default\] run every 15 seconds. This loops through all players and runs a series of actions based upon which options are enabled. By default, all below are enabled.

#### Give Custom Item

Gives players a custom item if they do not have one they own in their inventory. This uses the same function as on [player join](inventory-management.md#give-custom-item).

#### Remove Illegal Items

This loops through player's inventory and if they have a duplicated custom item or an item that does not belong to them, it will be deleted.

#### Update Custom Item

Updates the lore of a custom item. The same as [this](inventory-management.md#update-custom-item).

