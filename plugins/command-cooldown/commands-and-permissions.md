---
description: List of commands and permissions
---

# Commands & Permissions

### Base Command - /cc

Permission: commandcooldown.admin

| **Command** | **Description** | Permission |
| :--- | :--- | :--- |
| /cc help \[page\] | Shows a help list | commandcooldown.command.help |
| /cc list | Shows a list of all cooldowns | commandcooldown.command.list |
| /cc bypass | Bypasses all cooldowns | commandcooldown.command.bypass |
| /cc reload | Reloads the config.yml | commandcooldown.command.reload |
| /cc add | Enter the add command cooldown editor  | commandcooldown.command.add |
| /cc addalias | Enter the add alias editor | commandcooldown.command.addalias |
| /cc remove | Enter the remove command editor | commandcooldown.command.remove |
| /cc cancel | Exit all current editors | N/A |
| /cc \[addArguments/addArgs\] | Enter the add arguments editor | commandcooldown.command.addarguments |

### Other Commands

| Command | Description | Permission | Aliases |
| :--- | :--- | :--- | :--- |
| /cooldowns | Allows a player to see their active cooldowns | commandcooldown.cooldowns | cd |

### Other Permissions

<table>
  <thead>
    <tr>
      <th style="text-align:left">Permission</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">commandcooldown.bypass.command_here</td>
      <td style="text-align:left">Bypass a certain command with permission. Spaces are replaced with underscores</td>
    </tr>
    <tr>
      <td style="text-align:left">commandcooldown.<b>command</b>.<b>cooldown</b>
      </td>
      <td style="text-align:left">
        <p>Example: commandcooldown.home.30</p>
        <p>This would change the cooldown to 30 seconds for a player/group instead
          of the default for the command</p>
      </td>
    </tr>
  </tbody>
</table>

