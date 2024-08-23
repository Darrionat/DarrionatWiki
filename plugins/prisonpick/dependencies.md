---
description: Information about required/non-required plugins that PrisonPick can work with
---

# Dependencies

Dependencies are split up into 2 categories. Hard-dependencies, which are required, and soft-dependencies, which are not required, but offer extra features. \
\
As of now, PrisonPick has 2 hard dependencies, but they are not required for you to download them, as they are shaded within the plugin.jar itself. These shaded libraries are [XSeries](https://github.com/CryptoMorin/XSeries) and [NBTEditor](https://github.com/BananaPuncher714/NBTEditor). Although these are technically hard dependencies, you do not have to consider them at all if you are solely an administrator.\
\
PrisonPick also has a soft dependency on [TokenManager ](https://www.spigotmc.org/resources/tokenmanager.8610/)and an expansion for [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/). For detailed information on the PAPI expansion, [click here](placeholders.md).

{% content-ref url="placeholders.md" %}
[placeholders.md](placeholders.md)
{% endcontent-ref %}

### TokenManager

TokenManager is an economy plugin that PrisonPick can use for upgrading [enchantments](enchantments.md). This will replace the default currency of EXP levels. This can be enabled in the [config.yml](configuration-files/config.yml-1.0.2.md).\
[https://www.spigotmc.org/resources/tokenmanager.8610/](https://www.spigotmc.org/resources/tokenmanager.8610/)

### Vault

Vault is an economy plugin that PrisonPick can use for upgrading enchantments.\
Download here: [https://www.spigotmc.org/resources/vault.34315/](https://www.spigotmc.org/resources/vault.34315/)

### XSeries

XSeries is a library that allows PrisonPick to be highly compatible with older versions. XSeries allows for things such as potion effects, enchantments, and mostly item types to be used without major exceptions or failures.&#x20;

### NBTEditor

NBTEditor is used to save data to a specific item. With this library, custom data can be easily saved to an item. For example, pickaxes can have a designated owner, preventing other players from using that pickaxe.
