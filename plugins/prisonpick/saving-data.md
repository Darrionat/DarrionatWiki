---
description: The different ways PrisonPick can store a player's data and statistics
---

# Saving Data

PrisonPick stores data in different ways depending on how it is configured. Enchantments can be fetched from the [NBT tag](saving-data.md#from-nbt-tag) of a custom item, the [local file](saving-data.md#local-file), or a [MySQL database](saving-data.md#mysql-database). The blocks mined statistic can only be fetched from the local file or a MySQL database.

### Local File

A player's data is **always** saved locally, and that file can be found within `/plugins/PrisonPick/data/playerUUID.yml`This does not mean that data is always fetched from it. 

### MySQL Database

If enabled in the [config.yml](configuration-files/config.yml-1.0.2.md), data will also be stored within a MySQL database.  
If data is saved to a database, all statistics will be fetched from the database, unless enchantments are fetched [from the item](saving-data.md#from-nbt-tag) instead. If there is an SQLException, data will be fetched from the local file instead.

### Enchantments

Enchantments are always stored in the NBT tag of a custom item and within their local file.

#### From NBT Tag

If the option `getEnchantsFromItem` is enabled within the [enchants.yml](configuration-files/enchants.yml-1.0.2.md), enchantments will be **always** fetched from the NBT tag of the item. This means that if a player loses their pickaxe or if the pickaxe is removed from their inventory, all enchantments will be reset for that player. By default, this is false, meaning that the enchantment level depends on the [local file](saving-data.md#local-file) and/or a database.

