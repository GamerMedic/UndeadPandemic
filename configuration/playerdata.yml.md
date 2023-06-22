# 👩🔧 playerData.yml

{% hint style="success" %}
The `playerData.yml` file is a storage file.
{% endhint %}

This file stores different sets of player data, such as zombie kills, and health settings.

The file will look like this:

```
player_name:
  zombie_kills: 0
  zombie_head_shots: 0
  health:
    thirst: 80
```

{% hint style="info" %}
This data is where PlaceholderAPI pulls the data from, so changing this will show if you are displaying a scoreboard.
{% endhint %}

If you try to change the parameter names (i.e. `zombie_kills`), then the plugin will register the parameter as missing and will create a new line. This will reset the count.

You can update the player's data, but this file is otherwise not configurable.

{% hint style="warning" %}
**FUTURE UPDATES**: This file may be converted into a JSON storage file in a future update.&#x20;

The data contained in this file would be converted automatically.
{% endhint %}
