# Thirst Settings

**`enable_thirst`**:

Nice and basic.

`true|false`

If set to false, the XP level bar will work as normal. Otherwise, the XP level bar will act as the thirst indicator.

{% hint style="info" %}
**This no longer applies from v2.6.0**

It is _**strongly recommended**_ to set `enable_thirst` to `false` if you have enabled [enchants or mob drop XP orbs](../../configuration/config.yml/enchant-settings.md).
{% endhint %}

**`dehydration_rate`**:

This settings dictates how quickly (in seconds) a player's thirst will reduce by 1%. It is set to 90 seconds by default, but you can set this to whatever you want. The higher this value is, the slower a player will become thirsty.

{% hint style="info" %}
_**Future Update**: Increasing/Decreasing thirst based on the player's current biome is being considered._&#x20;
{% endhint %}

**`dehydration_qty`**:

This setting forces a percentage of thirst to decrease each time thirst is updated. Minimum 1%, maximum 99%.

{% hint style="info" %}
This setting was implemented in v2.6.0
{% endhint %}

**`purify_water`**:

This setting allows for water to be purified in a cauldron. Setting `purify_water` to `false` will also prevent the player from collecting contaminated water. This setting is `true` by default.

{% hint style="info" %}
This setting was implemented in v2.6.0
{% endhint %}

**`consumables`**:

Consumables are vanilla items that the player can consume that will increase the thirst bar.

```
  APPLE: 2
  BEETROOT_SOUP: 50
  CARROT: 5
  GOLDEN_CARROT: 15
  HONEY_BOTTLE: 15
  MELON_SLICE: 10
  MILK_BUCKET: 75
  MUSHROOM_STEW: 50
  POTION: 75
  RABBIT_STEW: 50
  ROTTEN_FLESH: -15
  SUSPICIOUS_STEW: -10
  WATER_BOTTLE: 75
```

The number after the item is the value that is added to the players thirst bar, for example, eating an Apple will add 2% to the player's thirst bar.

Negative numbers will make the player more thirsty.
