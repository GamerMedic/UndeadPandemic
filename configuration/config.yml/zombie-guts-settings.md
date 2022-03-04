# Zombie Guts Settings

{% hint style="success" %}
Version 2.4.2 introduced a significant update to Zombie Guts which has resulted in an entirely new section in the config.yml file.
{% endhint %}

Zombie Guts allow players to hide from zombies in plain sight. By wearing Zombie Guts players are blending in with the smell of the zombies. Over time the zombie guts will decompose and eventually fall away from the player. The guts will also be destroyed if they are in contact with water, so don't bother putting them on in the rain or when going for a swim.

Zombie Guts, when stored, will not decompose, so if they're not being worn, they're not losing power.

**`enabled`**:

`true|false`

This is set to true by default. Setting to false will stop zombie guts from working in the game.

**`chance`**:

The `chance` option decides the percentage chance that zombie guts are dropped. This will default to 3% (given as `3`).

Valid values are `1 - 100`. `0` (zero) is not a valid option because this means that guts will never be dropped. If you don't want zombie guts to drop when a zombie is killed then set `enabled` to `false`.

**`timer`**:

The timer dictates how long it will take for the guts to decompose. The times set here are all in seconds. A minimum and maximum time must be set, and if one is not given, then the default value will be used.

`min:`

This is set to 5 by default. Setting a negative number would just be silly (and won't do anything, in case you want to try it).

`max:`

This is set to 120 by default.

**`fade_in_water`**:

`fade_in_water` determines whether or not the guts will be destroyed when exposed to water.

`enabled`:

`true|false`

This is set to `true` by default.

`multiplier`:

The multiplier will determine how quickly guts will be used in water.

{% hint style="warning" %}
<mark style="color:orange;">**This option does not work in v2.4.2 but was accidentally included in the config.yml file on release. It will work in future versions.**</mark>
{% endhint %}

{% hint style="info" %}
**Future versions will allow you to customise the zombie guts item and texture.**
{% endhint %}

And that's all, folks! This completes the Zombie Guts settings in the configuration file.
