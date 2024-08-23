# MySQL

Command Cooldown stores data locally by default. In particular, all cooldown data of players is stored in the plugin's `playerdata` folder.&#x20;

**What is stored in the database?** Two important things are stored in the database: The command a player has a cooldown for **AND** when that cooldown will end.

**Why is this helpful?** If you, the administrator, want cooldowns to apply across multiple servers linked through BungeeCord, you must use the database connection.&#x20;

Example: Assume Player1 has a cooldown on `/tpa` on Server1 that ends in 30 minutes. By default, if Player1 uses /tpa on Server2, then the player will have no cooldown, **BUT** if the plugin is using the database connection, then the player will not be able to run `/tpa` _only if Server2 also has a cooldown on_ `/tpa`_._&#x20;

The database connection can be enabled in the plugin's `config.yml` file. A full plugin restart is required once enabled.
