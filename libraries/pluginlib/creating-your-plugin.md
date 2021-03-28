---
description: The first step of adding this library to your project
---

# Creating Your Plugin

### The Plugin Class

The class that you want to represent your plugin needs to extend `me.darrionat.pluginlib.Plugin`. 

```java
package me.darrionat.fakeplugin.FakePlugin;

import me.darrionat.fakeplugin.ErrorManager();

import me.darrionat.pluginlib.ErrorHandler;
import me.darrionat.pluginlib.Plugin;

public class FakePlugin extends Plugin {

	public void initPlugin() {
	  // Initializes your command
		new FakeCommand(this);
	}

	public ErrorHandler getErrorHandler() {
		return new ErrorManager();
	}

	@Override
	public void onDisable() {
		
	}
}
```

Typically, when you extend JavaPlugin, you use `onEnable()` but the `Plugin` superclass does some things behind the scenes before it starts your plugin, so you need to use `initPlugin()` instead.

When your plugin is disabled, `onDisable()` will be run.

### Error Handlers

Every plugin is required to have an `ErrorHandler`. More information about the `ErrorHandler` interface can be found [here](errorhandler.md). 

