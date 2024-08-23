---
description: The different ways PrisonPick can store a player's data and statistics
---

# Saving Data

PrisonPick stores data in different ways depending on how it is configured. Enchantments can be fetched from the [NBT tag](saving-data.md#from-nbt-tag) of a custom item, the [local file](saving-data.md#local-file), or a [MySQL database](saving-data.md#mysql-database). The blocks mined statistic can only be fetched from the local file or a MySQL database.

### Local File

A player's data is **always** saved locally, and that file can be found within `/plugins/PrisonPick/data/playerUUID.yml`This does not mean that data is always fetched from it.&#x20;

### MySQL Database

If enabled in the [config.yml](configuration-files/config.yml-1.0.2.md), data will also be stored within a MySQL database.\
If data is saved to a database, all statistics will be fetched from the database, unless enchantments are fetched [from the item](saving-data.md#from-nbt-tag) instead. If there is an SQLException, data will be fetched from the local file instead.

### Enchantments

Enchantments are always stored in the NBT tag of a custom item and within their local file.

#### From NBT Tag

If the option `getEnchantsFromItem` is enabled within the [enchants.yml](configuration-files/enchants.yml-1.0.2.md), enchantments will be **always** fetched from the NBT tag of the item. This means that if a player loses their pickaxe or if the pickaxe is removed from their inventory, all enchantments will be reset for that player. By default, this is false, meaning that the enchantment level depends on the [local file](saving-data.md#local-file) and/or a database.

### The Sync Data Command

The `/prisonpick syncData [file/db] confirm` command is a very unique command and one that probably won't be used often. This command copies all existing data from the given location and also sets those values at the other. **It will not remove any other existing data, but it will overwrite pre-existing stats for a player.**&#x20;

{% hint style="info" %}
The `confirm` argument exists to protect users from running this command accidentally or using it incorrectly. It must be remembered that the location you specify will be the **FROM** and the location you don't specify will be the **TO**.&#x20;
{% endhint %}

**File to Database Sync Example**

You just enabled my database, but you've been running PrisonPick for quite some time, so a lot of my players have statistics. To minimize the number of workarounds you have to do, there's a command built directly for this. To copy the stats from the [local files](saving-data.md#local-file) found within the data folder to the database, you just type `/prisonpick syncData file confirm`.

#### Database to File Sync Example

You have a server that's been using PrisonPick and a MySQL database, and you are planning on setting up another server on your network that uses the same data as the other. It's not necessary if you are using a database, but highly recommended that you run the command `/prisonpick syncdata db confirm` on the newer server. This will sync the data from the database to this new server.\
\
Even though within this example the local files are not being used, if a database occurs, PrisonPick will use the local file instead, so making sure both are the same is good practice.

{% hint style="danger" %}
Take caution while using this command. Syncing data **will overwrite** data if the data is not the same.
{% endhint %}
