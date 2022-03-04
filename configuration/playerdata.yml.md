# playerData.yml

{% hint style="success" %}
The `playerData.yml` is a storage file.
{% endhint %}

This file stores the number of zombie kills and head shots that a player achieves from joining the game.

The file will look like this:

```
player_name:
  zombie_kills: 0
  zombie_head_shots: 0
```

{% hint style="info" %}
This data is where PlaceholderAPI pulls the data from, so changing this will show if you are displaying a scoreboard.
{% endhint %}

If you try to change the parameter names (i.e. `zombie_kills`), then the plugin will register the parameter as missing and will create a new line. This will reset the count.

You can update the player's scores, but this file is otherwise not configurable.

{% hint style="warning" %}
**FUTURE UPDATES**: This file will be converted into a JSON storage file in a future update.&#x20;

The data contained in this file will be converted automatically.
{% endhint %}
