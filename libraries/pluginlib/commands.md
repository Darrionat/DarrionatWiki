---
description: >-
  PluginLib offers a simple way to create your commands and handles a few errors
  in the process
---

# Commands

### Creating a Command

To create a command within your plugin, you can do the following

#### Add the command to your plugin.yml

```yaml
name: FakePlugin
author: Darrionat
main: me.darrionat.FakePlugin
description: A fake plugin with commands
version: 1.0.0
api-version: 1.13

commands:
  ban:
    usage: /<command>
```

### Create a BaseCommand

```java
package me.darrionat.fakeplugin.commands;

import org.bukkit.command.Command;
import org.bukkit.command.CommandSender;

import me.darrionat.pluginlib.Plugin;
import me.darrionat.pluginlib.commands.BaseCommand;

public class FakeCommand extends BaseCommand {

	public FakeCommand(Plugin plugin) {
		super(plugin);
	}

	@Override
	public String getCommandLabel() {
		return "ban";
	}

	@Override
	protected void runNoArgs(CommandSender sender, Command command, String label, String[] args) {
		/*
		 * Do stuff
		 */
	}
}
```

Since the class above has no subcommands defined, it will always simply just run the `runNoArgs`method.

### SubCommands

A SubCommand is defined as a command that uses the same label as its parent BaseCommand but it has a different first argument. 

For example, your plugin has the base command `/ban`. You can add subcommands such as `/ban list` or `/ban player`. 

#### Adding a SubCommand to your BaseCommand

To add a SubCommand to a BaseCommand, you can use `BaseCommand#addSubCommand(SubCommand)`.

```java
public FakeCommand(Plugin plugin) {
		super(plugin);
		addSubCommand(new FakeSubCommand(this, plugin));
}
```

#### Example of a SubCommand Class

```java
package me.darrionat.fakeplugin.commands;

import org.bukkit.command.CommandSender;

import me.darrionat.pluginlib.Plugin;
import me.darrionat.pluginlib.commands.BaseCommand;
import me.darrionat.pluginlib.commands.SubCommand;

public class FakeSubCommand extends SubCommand {

	public FakeSubCommand(BaseCommand parentCommand, Plugin plugin) {
		super(parentCommand, plugin);
	}
	
	@Override
	public String getSubCommand() {
		// /ban list
		return "list";
	}

	@Override
	public int getRequiredArgs() {
		/*
		 * /ban list <- one argument
		 * This should always be greater than or equal to 1
		 */
		return 1;
	}

	@Override
	public boolean onlyPlayers() {
		return false;
	}

	@Override
	protected void runCommand(CommandSender sender, String[] args) {
		/*
		 * Do stuff
		 */
	}
}
```

