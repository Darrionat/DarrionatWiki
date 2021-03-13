---
description: PrisonPick's optional expansion for PlaceholderAPI
---

# Placeholders

Using the external [PlaceholderAPI ](https://www.spigotmc.org/resources/placeholderapi.6245/)\(PAPI\) expansion for PrisonPick, different data can be fetched. Using a placeholder where a plugin parses a string for placeholders will result in the placeholders being replaced with the returned values.  
  
PrisonPick fetches the data that is returned based upon how the plugin is configured. For more information on saving data and configuration, [click here](saving-data.md).

### Installation

1. Download the expansion from here. \[Not yet published\]
2. Add this .jar file to the /plugins/PlaceholderAPI/expansions folder on the server
3. Restart PlaceholderAPI

### Placeholders

Currently, there are two different types of statistics that are supported: number of blocks mined and enchantment levels. Placeholder parameters are not case-sensitive.

{% hint style="info" %}
For enchantments with names that are longer than one word, use `_` to separate words within the placeholder.
{% endhint %}

{% tabs %}
{% tab title="Placeholders" %}
| Placeholder | Returned String |
| :--- | :--- |
| %prisonPick\_blocksMined% | Gets the player's statistic for total blocks mined with their custom item |
| %prisonPick\_enchantName% | Gets the player's level of the defined enchantment |
{% endtab %}

{% tab title="Examples" %}
| Input | Output |
| :--- | :--- |
| `Blocks Mined: %prisonPick_blocksMined%` | `Blocks Mined: 534` |
| `Jump Boost Level: %prisonPick_jump_boost%` | `Jump Boost Level: 3` |
{% endtab %}
{% endtabs %}

