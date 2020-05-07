---
description: Information about custom blocks
---

# Custom Blocks

## Custom Blocks

Custom blocks are a feature within Custom Enchants+ that allows users to open up a [GUI](guis.md) by right-clicking the block. Each custom block has its own material already assigned to it. Custom blocks can be placed down or removed within [commands](commands-and-permissions.md). Each custom block is directly correlated to a GUI. A custom block will not work if the world they are in is disabled.

![](../../.gitbook/assets/image%20%287%29.png)

### Types

| Custom Block | Material |
| :--- | :--- |
| [Anvil](guis.md#the-anvil) | ANVIL |
| [Enchanter](guis.md#the-enchanter) | ENCHANTING\_TABLE |
| [Tinkerer](guis.md#the-tinkerer) | CAULDRON |

### Placing & Removing

Each custom block has its own placement [command ](commands-and-permissions.md)and removal command. Custom blocks can not be removed by breaking them.

### Holograms

Custom Enchants+ has a soft dependency on Holographic Displays. This allows for holograms to be enabled or disabled. These holograms can be configured to an admin's liking within the [config.yml](configuration-files/config.yml.md). Holograms are reloaded with the command `/ce reload`

#### Enabling Holographic Displays

1. Add Holographic Displays to the server
2. Go into Custom Enchant's+ config.yml
3. Go the configuration section 'holograms' and set 'enabled' to true.
4. Save the config.yml
5. Restart your server

{% hint style="warning" %}
Note: Holograms will not work if you do not enable them within the config.yml of Custom Enchants+.
{% endhint %}

### Data Files

Each custom blocks has its own .yml file to be saved to.

| Custom Block | File Name |
| :--- | :--- |
| Anvil | anvilData.yml |
| Enchanter | tableData.yml |
| Tinkerer | tinkerData.yml |

