---
description: List of commands and their functionalities
---

# Commands

{% hint style="info" %}
All commands use the 'p!' prefix
{% endhint %}

### General Commands

These commands do not require any permissions

| Command                     | Description                                                                                                           |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| p!help \[Optional: command] | <p>p!help: Displays the list of commands</p><p>p!help [command]: Gives information about a specified command</p>      |
| p!invite                    | Gives a link to invite the bot to a server                                                                            |
| p!ping                      | Returns the bot's ping                                                                                                |
| p!plugin \[resource\_id]    | Gives information about a specific resource                                                                           |
| p!stats                     | Shows some bot statistics                                                                                             |
| p!wiki                      | Sends a link to this wiki                                                                                             |
| p!search \[resource\_name]  | Searches for the top resources with the given name. Use -n \[size] at the end of the command to increase search size. |

### Administrator Commands

These commands all require the Administrator permission

| Command                           | Description                                                                     |
| --------------------------------- | ------------------------------------------------------------------------------- |
| p!add \[resource\_id] \[#channel] | Starts to watch for plugin updates and will post updates in the defined channel |
| p!list                            | Gives a list of watched resources and their channels to post in                 |
| p!remove \[resource\_id]          | Stops watching a resource in its defined channel                                |
