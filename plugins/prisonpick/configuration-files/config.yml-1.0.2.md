---
description: 1.0.2
---

# config.yml

{% hint style="danger" %}
Within the config.yml the material of the pickaxe can be changed to any material. However, it is **highly recommended** to **ONLY** use a pickaxe material. Using a different material such as _OAK\_LOG_ could potentially lead to unexpected bugs or effects, mainly with enchantments.\
\
If you experience a bug by using a non-pickaxe material, you may make a bug report, but do not expect functionality to come to a specific item.
{% endhint %}

{% hint style="info" %}
Within the custom item lore, the placeholder %owner% can be used to display the owner's username, and %minedBlocks% can be used to show the mined block stat of the owner.
{% endhint %}

```
pickaxe:
  # The name of the pickaxe, %player% will be replaced with the owner's name
  name: '&6%player%s &ePickaxe'
  slot: 0
  material: DIAMOND_PICKAXE
  # Determines whether to set the pickaxe to unbreakable or not
  unbreakable: true
  lore:    
    lines:
      - '&2&lStatistics'
      - '&aOwner &b%owner%'
      - '&aBlocks mined &b%minedBlocks%'
      - ''
      - '%enchantmentsSection%'
    # Enchantments section can be inserted into the lore with the
    # %enchantmentsSection% placeholder
    # If a line contains this placeholder, it will be replaced with the lines below
    enchantmentsSection:
      headerEnabled: true
      header: '&c&lEnchantments'
      enchant: "&e%enchantName% &f%enchantLevel%"
# TokenManager support. This must be true to set TokenManager as the main economy
tokenManager:
  enabled: false
  # How prices are displayed
  display: '&f%tokens% Tokens'
# How prices are displayed
experience:
  display: '&f%expLevels% Levels'
# The amount of upgrade an enchantment by based upon the type of click
enchantLevelUpgrade:
  leftClick: 1
  rightClick: 10
  shiftRightClick: 100
# Inventory Options
inventory:
  # If false, will prevent a player from moving the pickaxe in their inventory
  allowMovePickaxe: false
  # If false, will not let player drop the custom item
  allowDropPickaxe: false
  # If false, will not drop custom item on death
  dropPickaxeOnDeath: false
  givePickaxeOnJoin: true
  # If true, this will completly delete the item that was in the pickaxe's assigned slot;
  # otherwise, move the item into a different slot or drop naturally
  replaceItemInHotbarSlot: false
  # Updates the pickaxe's lore or NBT tags
  updatePickaxeOnJoin: true
  # A timer that is ran 
  timer:
    enabled: true
    # The amount of seconds between each time the timer runs
    seconds: 15
    # Removes pickaxes that do not belong to the player
    # Also removes duplicated pickaxes
    removeIllegalPickaxes: true
    # Gives a player a pickaxe if they don't have one that they own in their inventory
    givePickaxe: true
    # Updates the lore or NBT tags of the pickaxe
    updatePickaxe: true
blockBreak:
  # Puts items directly into a player's inventory
  itemsToInventory: true
  # If true, doesn't drop EXP on the ground, but gives it to player instead
  autoPickupExp: true
# GUI settings
pickaxeGui:
  name: 'Pickaxe'
  rows: 5
  fillItemMaterial: BLACK_STAINED_GLASS_PANE
# Database support
mysql:
  enabled: false
  host: localhost
  port: 3306
  database: name
  username: root
  password: password
```
