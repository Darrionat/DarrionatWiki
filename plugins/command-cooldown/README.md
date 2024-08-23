---
description: >-
  The best plugin for adding cooldowns to commands and preventing spam! 1.7-1.21
  support!
---

# Command Cooldown

![](../../.gitbook/assets/Command-Cooldown-Banner1.png)



## Description

Command Cooldown is an administrative plugin for Minecraft servers (support for Bukkit/Spigot and BungeeCord). Administrators can create cooldowns that will make a player wait before they can execute a certain command again. Command Cooldown can be used to help prevent spam as well.

## Plugin Downloads & Changelogs

Spigot MC: [https://www.spigotmc.org/resources/command-cooldown.73696/](https://www.spigotmc.org/resources/command-cooldown-1-7-1-15-support-add-cooldowns-to-commands.73696/)\
DevBukkit: [https://dev.bukkit.org/projects/command-cooldowns](https://dev.bukkit.org/projects/command-cooldowns)

## Features

* Place a cooldown on **ANY** command!
* Sync cooldowns through BungeeCord with our **MySQL** Support
* Edit command cooldowns in a GUI editor `/cc editor`
* See your current cooldowns `/cc cooldowns`
* See other player's current cooldowns `/cc cooldowns UUID/playerName`
* Bypass cooldowns with a command `/cc bypass`
* Bypass cooldowns with permissions `commandcooldown.bypass.command_here`. Example: `commandcooldown.bypass.warp_shop`
* Remove all current cooldowns `/cc removecooldowns playerName`
* Automatic **time formatting** in plugin messages and the GUI Editor
* Customizable messages in **messages.yml**
* Automatically checks for updates
* Automatically updates config.yml every new update
* Add aliases to commands! Example: `/cc` and `/commandcooldown` are aliases for the same command
* Text prompts to help create Command Cooldowns
* Automatic time formatting `(s=seconds, m=minutes, h=hours, d=day, w=week, y=year)`.
* Change cooldowns via permissions. Example: `commandcooldown.warp_home.30` will set the player's default cooldown for `/warp home` to 30 seconds.

{% content-ref url="commands-and-permissions.md" %}
[commands-and-permissions.md](commands-and-permissions.md)
{% endcontent-ref %}

{% content-ref url="configuration-files/" %}
[configuration-files](configuration-files/)
{% endcontent-ref %}

{% content-ref url="mysql.md" %}
[mysql.md](mysql.md)
{% endcontent-ref %}

{% content-ref url="trivia.md" %}
[trivia.md](trivia.md)
{% endcontent-ref %}
