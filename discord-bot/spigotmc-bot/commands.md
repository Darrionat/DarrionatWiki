---
description: List of commands and their functionalities
---

# Commands

{% hint style="info" %}
All commands use the 'p!' prefix
{% endhint %}

### General Commands

These commands do not require any permissions

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">p!help [Optional: command]</td>
      <td style="text-align:left">
        <p>p!help: Displays the list of commands</p>
        <p>p!help [command]: Gives information about a specified command</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">p!invite</td>
      <td style="text-align:left">Gives a link to invite the bot to a server</td>
    </tr>
    <tr>
      <td style="text-align:left">p!ping</td>
      <td style="text-align:left">Returns the bot&apos;s ping</td>
    </tr>
    <tr>
      <td style="text-align:left">p!plugin [resource_id]</td>
      <td style="text-align:left">Gives information about a specific resource</td>
    </tr>
    <tr>
      <td style="text-align:left">p!stats</td>
      <td style="text-align:left">Shows some bot statistics</td>
    </tr>
    <tr>
      <td style="text-align:left">p!wiki</td>
      <td style="text-align:left">Sends a link to this wiki</td>
    </tr>
  </tbody>
</table>

### Administrator Commands

These commands all require the Administrator permission

| Command | Description |
| :--- | :--- |
| p!add \[resource\_id\] \[\#channel\] | Starts to watch for plugin updates and will post updates in the defined channel |
| p!list | Gives a list of watched resources and their channels to post in |
| p!remove \[resource\_id\] | Stops watching a resource in its defined channel |

