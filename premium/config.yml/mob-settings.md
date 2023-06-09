# Mob Settings

Mob settings is where you can decide what mobs will still appear in your worlds, and this is where zombie spawning is controlled.

**`disable_mobs`**:

Use this setting to list what mobs that you _**do not**_ want to appear in your world. You must use the official Minecraft Entity names in this setting.

{% hint style="info" %}
_**RESOURCE**_: You can [find the mob entity names right here](https://papermc.io/javadocs/paper/1.16/org/bukkit/entity/package-summary.html).
{% endhint %}

This is the default mobs list:

```
disable_mobs:
  - BLAZE
  - CAVE_SPIDER
  - CREEPER
  - ENDER_DRAGON
  - ENDERMAN
  - ENDERMITE
  - EVOKER
  - EVOKER_FANGS
  - EVOCATION_ILLAGER
  - EVOCATION_FANGS
  - GHAST
  - GIANT
  - HUSK
  - PHANTOM
  - PILLAGER
  - RAVAGER
  - SKELETON
  - SLIME
  - SPIDER
  - STRAY
  - STRIDER
  - VEX
  - VINDICATOR
  - VINDICATION_ILLAGER
  - WITCH
  - WITHER
  - WITHER_SKELETON
```

The mobs above will not appear in the world. You can remove, or comment out, the mobs that you would like to appear in your world. You can comment them out by putting a hash (#) in front of the hyphen (-), like so:

```
# - BLAZE
```

{% hint style="warning" %}
The below settings have been moved to [Zombie Settings](../../configuration/config.yml/zombie-settings.md).
{% endhint %}

&#x20;**`zombie_spawn_rate`**:

You can determine how many zombies will spawn in the world using this setting.

{% hint style="danger" %}
&#x20;                                                   _<mark style="color:red;">**BE CAREFUL WITH THIS SETTING!**</mark>_
{% endhint %}

The higher this value is, the more likely it is that your server will lag. If you set this too high, you could crash your server. For this reason, this setting is limited to within the range of `1 - 25`, though even 25 is quite risky (and unnecessary!).

This setting works by multiplying the number of naturally spawned zombies by the `zombie_spawn_rate`. So a `zombie_spawn_rate` of 1 is the default Minecraft behaviour, which means that if the `zombie_spawn_rate` is set to 5, then an addition 4 zombies will spawn when one spawns naturally.

**`attract_zombie_rate`**:

This is the number of zombies that will appear when a gun is fired. The acceptable range for this setting is `0 - 25`. Again, you should be careful with this setting as it can cause lag.

**`attract_zombie_radius`**:

This is the radius (in blocks) in which zombies will appear after a gun is fired. It's set to 5 by default, but can be set to anything you want. Anything too high and your players will never see the zombies. You want this to be fairly close to the player, and just far enough that players will not have zombies spawn on top of them.

**`attract_zombie_chance`**:

This is the percentage chance that a zombie will hear gun fire. Setting this to 100 will guarantee that zombies will hear gun fire.

This option can be set to from between `0 - 100`.

0 will mean that no zombies will appear.

