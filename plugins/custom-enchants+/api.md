---
description: Information about the API for Custom Enchants+
---

# API

## How to utilize CustomEnchants+'s API

{% hint style="info" %}
All API methods can be found [HERE](https://github.com/Darrionat/CustomEnchantsAPI/blob/master/CustomEnchantsAPI.java)
{% endhint %}

Within your plugin.yml add

```text
softdepend: [CustomEnchantsPlus]
```

If you want CustomEnchants+ to be absolutely necessary to your plugin do this instead

```text
depend: [CustomEnchantsPlus]
```

#### Add CustomEnchants+ to your Java Project as an external library

#### Utilize the API by using the static methods within CustomEnchantsAPI

Example:

```text
CustomEnchantsAPI.openGui(player, CustomEnchantGui.ENCHANTER);
```

#### Obtaining a specific custom enchantment

Example:

```text
Enchantment enchant = CustomEnchantment.EXPLOSIVE_ARROW;
```

#### Obtaining a scroll

Example:

```text
Scroll scroll = Scrolls.ENCHANTMENT_REMOVAL;
```

