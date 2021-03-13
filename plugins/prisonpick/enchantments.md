---
description: Information about pickaxe enchantments
---

# Enchantments

Enchantments can be added through the [Pickaxe GUI](). Enchantments must all have a defined cost, slot of where they are displayed in the GUI, max level, and display information. Enchantments can also have other settings within the [enchants.yml](configuration-files/enchants.yml-1.0.2.md) depending on what they inherit. All enchantments have a minimum level of 1 and must have a unique name.

## Vanilla Enchantments

Custom enchantments that extend the VanillaEnchantment class add a vanilla enchantment to the item based upon what level the custom enchantment is. This is based upon a setting called `levelsPerVanillaLevel`. The level of the vanilla enchantment is calculated as follows:  
  
**Example**:  
`levelsPerVanillaLevel: 30  
Custom enchant level = 65  
65/30 = 2.17 -> 2`  
_Always rounded down as an integer_

### Efficiency

Efficiency increases the speed at which the tool can mine. The mining speed is fully based upon that of the vanilla enchantment and does not use unique attributes, packets, etc.

#### Enchantment Information

| Default Max Level | Default levels/vanilla level |
| :--- | :--- |
| 100 | 20 |

### Fortune

Fortune increases the number of drops that a player can get from certain ores and materials. The vanilla fortune calculation is actually canceled and PrisonPick does its own calculation that is the exact same. This is because Spigot API was not consistent across versions, so I had to create my own loot table. All calculations are the exact same as those on [this page](https://minecraft.gamepedia.com/Fortune).

{% hint style="info" %}
The custom calculation of Fortune will not affect the calculation of non-custom items.
{% endhint %}

#### Currently Supported Ores 

| Ore |
| :--- |
| Coal Ore |
| Nether Quartz |
| Diamond Ore |
| Emerald Ore |
| Nether Gold Ore |
| Lapis Lazuli |
| Redstone |

#### Enchantment Information

| Default Max Level | Default levels/vanilla level |
| :--- | :--- |
| 100 | 20 |

## Potion Enchantments

Potion enchantments give a particular potion effect when the custom item is held. All potion effects given by an enchantment have an unlimited duration. The level of the potion also depends on the level of the custom enchantment. This is calculated by a setting called `levelsPerPotionLevel`. The level of the potion is calculated as follows:  
  
**Example**:  
`levelsPerPotionLevel: 2  
Speed enchant level = 3  
3/2 = 1.5 -> Speed 1`  
_Always rounded down as an integer_

{% hint style="info" %}
Potion effects are added when a player switches their current item to the pickaxe. So if you just upgraded the enchantment and you don't have the effect, try switching items.
{% endhint %}

### Haste

The custom enchantment of Haste gives the potion effect [Haste](https://minecraft.gamepedia.com/Haste). This will increase how fast the player digs.

| Default Max Level | Default levels/potion level |
| :--- | :--- |
| 5 | 1 |

### Speed

The custom enchantment of Speed gives the potion effect [Speed](https://minecraft.gamepedia.com/Speed). This will increase how fast the player runs. 

{% hint style="info" %}
This enchantment may not be a potion enchantment in the future, but rather, it may change the attribute of the player's walking speed. - This will depend on user feedback.
{% endhint %}

| Default Max Level | Default levels/potion level |
| :--- | :--- |
| 5 | 1 |

### Jump Boost

The custom enchantment of Jump Boost gives the potion effect [Jump Boost](https://minecraft.gamepedia.com/Jump_Boost). This will change how fast the player can jump.

| Default Max Level | Default levels/potion level |
| :--- | :--- |
| 4 | 1 |

### Night Vision

The custom enchantment of Night Vision will give the potion effect [Night Vision](https://minecraft.gamepedia.com/Night_Vision). This will change how easily the player can see in the dark. 

{% hint style="warning" %}
Setting the max level of this enchantment to higher than 1 will do nothing unless you also change the default levels/potion level. Doing this would mean the player needs to upgrade the enchantment enough times to actually get the potion effect; however, this is not recommended. It is recommended that you instead, increase the price of this enchantment and keep the default max level as 1.
{% endhint %}

| Default Max Level | Default levels/potion level |
| :--- | :--- |
| 1 | 1 |

