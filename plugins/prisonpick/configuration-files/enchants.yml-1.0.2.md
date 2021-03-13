---
description: 1.0.2
---

# enchants.yml

```text
enchantData:
  # This determines where the enchantment data will be fetched from. Having this set to false will 
  # mean that player's enchantments will be determined from their saved data (config file or database). 
  # However, if true, the enchantments will be fetched from the NBT tag of the item.
  getEnchantsFromItem: false
clickTypeAmount:
  leftClick: 1
  rightClick: 10
  shiftRightClick: 100
  middleClick: MAX
guiLore:
  - '%description%'
  - ''
  - '&eCurrent Level &f%currentLevel%/%maxLevel%'
  - '&ePrice &f%price%'
  - ''
  - '&fLeft-Click &7To Add &f%leftClickAmount% &7Level'
  - '&fRight-Click &7To Add &f%rightClickAmount% &7Levels'
  - '&fShift Right-Click &7To Add &f%shiftRightClickAmount% &7Levels'
  - '&fMiddle-Click &7To Add &f%middleClickAmount% &7Levels'
efficiency:
  maxLevel: 100
  levelsPerVanillaLevel: 20
  gui:
    slot: 28
    cost: 50
    material: DIAMOND_PICKAXE
    displayName: '&e&lEFFICIENCY'
    description: '&fMine blocks faster'
fortune:
  maxLevel: 100
  levelsPerVanillaLevel: 20
  gui:
    slot: 29
    cost: 50
    material: EMERALD
    displayName: '&a&lFORTUNE'
    description: '&fMultiply the amount of drops you mine'
haste:
  maxLevel: 5
  levelsPerPotionLevel: 1
  gui:
    slot: 30
    cost: 50
    material: FEATHER
    displayName: '&6&lHASTE'
    description: '&fGain levels of haste'
speed:
  maxLevel: 5
  levelsPerPotionLevel: 1
  gui:
    slot: 32
    cost: 50
    material: SUGAR
    displayName: '&e&lSPEED'
    description: '&fGain levels of speed'
jumpBoost:
  maxLevel: 4
  levelsPerPotionLevel: 1
  gui:
    slot: 33
    cost: 50
    material: RABBIT_FOOT
    displayName: '&a&lJUMP BOOST'
    description: '&fAbility to jump higher'
nightVision:
  maxLevel: 1
  levelsPerPotionLevel: 1
  gui:
    slot: 34
    cost: 50
    material: ENDER_EYE
    displayName: '&d&lNIGHT VISION'
    description: '&fGain night vision'
```

