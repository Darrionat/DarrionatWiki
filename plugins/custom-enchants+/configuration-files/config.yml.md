# config.yml

```text
checkUpdates: true
checkLoreUpdates: true
EnchantGUI Name: Enchanter
TinkerGUI Name: Tinker
AnvilGUI Name: Anvil
selectEnchantGuiName: 'Select an enchantment'
EnchanterEnabled: true
TinkererEnabled: true
AnvilEnabled: true
OnlyCustomAnvil: false
OnlyCustomEnchantmentTable: false
OnlyCustomCauldron: false

defaultMaxSlots: 3
enchantExpCost: 40
forgeExpPerEnchantment: 15
enabledWorlds:
- world
- world_nether
- world_the_end
upgradeExistingEnchantsOnEnchant:
  enabled: true
  percent: 50
rarity:
  normalPercentage: 95
  rarePercentage: 4
  legendaryPercentage: 1
vanillaEnchantmentTable:
  buttonPercentagesForCustomEnchant:
    1: 25
    2: 50
    3: 75
holograms:
  enabled: false
  addItemLine: true
  anvil:
    - '&cForge &7your &dCustom Enchants'
    - '&7together within &cThe Anvil'
  enchanter:
    - '&dEnchant &7your weapons, armor'
    - '&7and tools with &dcustom enchantments'
    - '&7in &dThe Enchanter'
  tinker:
    - '&eSacrafice &7your enchantments for'
    - '&eexperience &7in &eThe Tinkerer'
scrolls:
  enchantmentRemovalScroll:
    percentage: 5
    material: REDSTONE
    name: '&cEnchantment Removal Scroll'
    lore:
      - '&7Drag and drop this on to a custom &denchanted &7item to'
      - '&7choose an &dEnchantment &7to &cremove permanently.'
  enchantmentUpgradeScroll:
    material: EMERALD
    percentage: 5
    name: '&aEnchantment Upgrade Scroll'
    lore:
      - '&7Drag and drop this on to a custom &denchanted &7item to'
      - '&7choose an enchantment &aupgrade.'
  slotUpgradeScroll:
    material: PAPER
    percentage: 5
    name: '&aSlot Upgrade Scroll'
    lore:
      - '&7Drag and drop this on to a custom &denchanted'
      - '&7item to get &a+1 Slot&7.'
  itemRepairScroll:
    material: ANVIL
    percentage: 5
    name: '&cItem Repair Scroll'
    lore:
      - '&7Drag and drop this on to a custom &denchanted &7item'
      - '&7to &creapir &7all durability'
  renamingScroll:
    material: NAME_TAG
    percentage: 5
    name: '&eRenaming Scroll'
    lore:
      - '&7Drag and drop this on to a custom &denchanted'
      - '&7item to &erename &7it.'
enchantmentToken:
  material: SUNFLOWER
  name: '&dEnchantment Token &7- %enchantment%'
  lore:
    - '&7Drag and drop this on to any item you want to apply'
    - '&7the &denchantment &7on to. Only works with compatible'
    - '&eitems &7and &denchantments&7.'
wand:
  crafting:
    enabled: true
  material: BLAZE_ROD
  name: '&dMystical Wand'
```

