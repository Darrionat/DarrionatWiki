# autosell.yml

{% hint style="warning" %}
To create a rank, it needs to be underneath the configuration section `prisonpick.rank`.
{% endhint %}

```text
# The autosell.yml file defines what blocks sell for what prices.
# 
# Since most prison servers function by groups and ranks, different permissions can have different prices
#
# Instead of depending on multiple permission plugins, PrisonPick looks at the permissions of a player instead.
# 
# For example, if a player has the permission prisonpick.rank.a and that permission has DIAMOND_BLOCK 
# for 50 (type of currency), then the player will be given 50 of the configured currency.
# 
# These permissions must be in the format `prisonpick.rank.{GROUP}`
# 
# If a player has more than one of the following permissions, and a certain item is found in both, 
# the player will be sold the higher priced item.

prisonpick.rank:
  a:
    DIAMOND_BLOCK: 500
    EMERALD_BLOCK: 750
  b:
    DIAMOND_BLOCK: 750
    EMERALD_BLOCK: 1000
```

