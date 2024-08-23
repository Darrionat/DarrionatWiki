# Configuration Files

All config files can be customized to a high degree. They will be automatically saved if the files do not already exist when the plugin is initialized. \
All messages can be configured as well.\
When the reload command is run, the configuration services within the plugin will automatically reload all settings from the configs.

{% hint style="warning" %}
Files that save data are not considered to be a config file, look at [this page](../saving-data.md) for data files
{% endhint %}

### Auto Update

All configuration files will be automatically updated to include all settings, remove settings that no longer exist, and the version will also be in the config.\
\
**Why does this matter?**\
The configs do not need to be deleted/recreated in order to get the newer settings.\
Configs do not need to be deleted and recreated in order to delete outdated settings.\
If there is a bug, it is easy for the developer to find out what version you are using by looking at your configuration files.\
\
**The disadvantage of Automatic Updates**\
Unless specified, the updater will remove all comments. This is due to how the Spigot API handles YAML configurations, they do not save comments along with the data. I'm still looking for a workaround and there should be a fix to this in the future; however, it's not on the top of my to-do list.\
This single disadvantage is not large enough for me to remove the updater due to its incredible usefulness.

{% content-ref url="config.yml-1.0.2.md" %}
[config.yml-1.0.2.md](config.yml-1.0.2.md)
{% endcontent-ref %}

{% content-ref url="enchants.yml-1.0.2.md" %}
[enchants.yml-1.0.2.md](enchants.yml-1.0.2.md)
{% endcontent-ref %}

{% content-ref url="messages.yml-1.0.2.md" %}
[messages.yml-1.0.2.md](messages.yml-1.0.2.md)
{% endcontent-ref %}
