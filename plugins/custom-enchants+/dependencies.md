---
description: Integration with other plugins
---

# Dependencies

#### Enabling **a Dependency**

1. Add the plugin to the server
2. Go into Custom Enchant's+ config.yml
3. Go the configuration section `holograms`,  `towny`, or `worldguard` and then set 'enabled' to true.
4. Save the config.yml
5. Restart your server

{% hint style="warning" %}
Note: A dependency will not integrate properly if you do not enable it within the config.yml of Custom Enchants+
{% endhint %}

### HolographicDisplays

Custom Enchants+ has a soft dependency on Holographic Displays. This allows for holograms to be enabled or disabled. These holograms can be configured to an admin's liking within the [config.yml](configuration-files/config.yml.md). Holograms are reloaded with the command `/ce reload` These holograms can be seen with [Custom Blocks](custom-blocks.md)

### **Towny**

Towny integration can add protection and function properly with claims made through Towny. If a player is in a town, it will check to see if they are in a plot. If they are, it will check to see if they have permission, and if they aren't it will check to see if they are a resident of the town. _If the player is the owner, a resident, or a friend of the plot owner, they are able to use custom enchantments within the plot._

### WorldGuard

All enchantments can be disabled through WorldGuard using the flag 'custom-enchants'.  
To add this flag, just run the command: **/rg flag \[region name\] custom-enchants \[deny/allow\]**

