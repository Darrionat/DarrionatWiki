---
description: Integration with other plugins
---

# Dependencies

#### Enabling **a Dependency**

1. Add the plugin to the server
2. Go into Custom Enchant's+ config.yml
3. Go to the configuration section `holograms` and then set 'enabled' to true.
4. Save the config.yml
5. Restart your server

{% hint style="warning" %}
Note: A dependency will not integrate properly if you do not enable it within the config.yml of Custom Enchants+
{% endhint %}

### HolographicDisplays

Custom Enchants+ has a soft dependency on Holographic Displays. This allows for holograms to be enabled or disabled. These holograms can be configured to an admin's liking within the [config.yml](configuration-files/config.yml.md). Holograms are reloaded with the command `/ce reload` These holograms can be seen with [Custom Blocks](custom-blocks.md)

### Event Compatability

All [enchantments ](enchants.md)function on certain events. However, CustomEnchants+ forces Bukkit to run the events within CustomEnchants+ later than other plugins, so CustomEnchants+ will not fire enchantment events if another plugin cancels them first. This is good for allowing plugins that have protected regions such as WorldGuard or a Skyblock plugin to prevent a player from using enchantments within that area.

