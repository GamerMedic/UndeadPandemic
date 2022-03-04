# Infection Settings

Okay, so here's where things get really exciting.

The infection settings dictate if a player can be infected, how long they will be infected for, how severe infections will be, and whether to amplify damage while keeping ill effects at bay or not.

**`enabled`**:

Whether or not to enable zombie bite infections.

`true|false`

This is `true` by default.

**`infection_symptoms`**:

This is a list of buffers that will be applied to the player when they are infected by a zombie. These buffers should be listed using the `PotionEffectType` given by the [Spigot API](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionEffectType.html).

The default list is:

```
- POISON
- HARM
- SLOW
- SLOW_DIGGING
- HUNGER
- INCREASE_DAMAGE
- DAMAGE_RESISTANCE
```

**`duration`**:

How long should the effects of infection last? This is set in seconds, and is set to 120 seconds by default.

Damage is part of the zombie infection, which means that, if set for long enough, the zombie infection will kill the player unless they are cured before they die.

**`amplifier`**:

The amplifier settings will determine how severe the symptoms of the zombie infection are. The smaller this number is, the less effect infection will have on a player, i.e. they won't receive much damage. The higher this number is, the more intense the player's experience is.

You can't use negative numbers here, and very high numbers may cause lag.

The default value is 10.

**`amplify_effect`**:

This will determine how the infection will affect players.

`damage_only|all`

Setting this option to `damage_only` will apply the `amplifier` value only to the damage effects to the player. All other infection symptoms will be amplified by 10.

`all` will amplify all symptoms equally.

**`cure_with_milk`**:

This option determines whether or not players can cure buffers with milk. This is the vanilla Minecraft action of milk. UndeadPandemic will disable curing buffers with milk by default.

`true|false`

This is `false` by default.
