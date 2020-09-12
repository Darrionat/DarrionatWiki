---
description: Default for example
---

# cooldowns.yml

```text
# The label (base) of the command
tpa:
  # Where the cooldowns are defined
  cooldowns:
    # This * symbol must be here! This is the base cooldown for the entire command.
    # Set this cooldown to 0 if you only want cooldowns on certain arguments
    *: 60
    # These are the arguments
    Notch: 30
    Darrionat: 30
  # Aliases are labels that can also trigger the cooldown. I.g. /factions and /f
  aliases:
    - etpa
    - tpahere
repair:
  cooldowns:
    *: 30
    hand: 20
    abc *: 50
    abc d: 40
  aliases:
    - repairs
```

