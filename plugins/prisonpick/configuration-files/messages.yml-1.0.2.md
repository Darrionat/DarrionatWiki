---
description: 1.0.2
---

# messages.yml

```text
prefix:
  enabled: true
  prefix: '&7[&6Prison Pick&7]&f '
errors:
  notEnoughMoney: '&cYou do not have enough to afford this enchantment'
  onlyPlayers: '&cOnly players can send that command!'
  noPermission: '&cYou do not have the permission %permission%!'
  playerNotOnline: '&cThat player is not online!'
  invalidEnchant: '&cThat is an invalid enchantment'
  notANumber: '&cThat is not a valid integer'
  notValidLevel: '&cNot a valid level! Send a level from 0 to %maxLevel%'
messages:
  pickaxeRemoved: '&aSuccessfully removed %player%s pickaxe'
  setEnchantment: '&aSuccessfully set &e%player%s &aenchantment &e%enchantment% &ato level &e%level%'
  resetPlayer: '&aSuccessfully &creset &aall enchantments from &e%player%'
  toggleBypass: '&aBypassing set to &e%status%'
  reloaded: '&aSuccessfully reloaded all files and settings'
commandMessages:
  baseMessages:
    - '&7[&6Prison Pick&7] &7Author: &6Darrionat'
    - '  &7Type &6/pp help &7for more information'
  help:
    header: '&6Help Page &f%page%&7/&f%pageAmount%'
    help: '&6/pp help [page] &7- More command information'
    helpgui: '&6/pp helpgui &7- Opens a Gui that contains more command information'
    removePickaxe: '&6/pp removePickaxe [player] &7- Removes a players item'
    setEnchant: '&6/pp setEnchant [player] [enchant] [level] &7- Sets a players level for a particular enchantment'
    syncData: '&6/pp syncData [file/db] confirm &7 - Syncs the data from the selected data location to the other'
    resetPlayer: '&6/pp resetPlayer [player] &7- Resets &call &7of a players enchantments to &a0'
    bypass: '&6/pp bypass &7- Allows a player to be able to move a pickaxe in their inventory'
    reload: '&6/pp reload &7- Reloads all config files and settings'
```

