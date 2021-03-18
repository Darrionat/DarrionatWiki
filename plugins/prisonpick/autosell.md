---
description: Detailed information on how Autosell works
---

# Autosell

Autosell is a feature that allows a player to automatically sell their items for whatever type of economy the plugin uses. The player is able to automatically sell items if the option is enabled within the [config.yml](configuration-files/config.yml-1.0.2.md). Autosell can be used when blocks [go directly to a player's inventory](inventory-management.md#blocks-to-inventory) or it can be used via a timer.

### Ranks

A rank gives a player access to a set of selling [prices](autosell.md#prices).   
Ranks can be created within the [autosell.yml](configuration-files/autosell.yml.md) file. Ranks have names that will not be displayed, but they should be seen in a player's permissions. 

#### Giving a Player a Rank

To give a player a rank, you must give them the permission `prisonpick.rank.rankName`.

{% hint style="info" %}
If a player has multiple ranks, and two or more have a price for the same item, the highest selling price will be used.
{% endhint %}

### Prices

A price is a combination of a selling material and a sell value. To set a price for a rank, within the [autosell.yml](configuration-files/autosell.yml.md), you can add a price by adding `itemtype: sellPrice` to the rank's config section.  
If there is an invalid material, a warning will be printed in the console and the item will not be taken into account.  
For the full list of valid item types, click [here](https://github.com/CryptoMorin/XSeries/blob/master/src/main/java/com/cryptomorin/xseries/XMaterial.java).

