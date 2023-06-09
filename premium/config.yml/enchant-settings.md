# Enchant Settings

There are two configuration options for enchants.

{% hint style="warning" %}
It is _**strongly recommended**_ to disable the [thirst system](../../configuration/config.yml/thirst-settings.md) if you have either of these settings enabled.

The thirst system will allow players to fill their XP bar by using consumables defined by the thirst system.
{% endhint %}

**`allow_enchants`**:

Should players be allowed to use the enchanting table? This is set to `false` by default because the thirst system is enabled by default. The thirst system uses XP levels to display thirst, and so is set high (up to 100) a part of the game play.

Allowing players to use the enchanting table while the thirst system is on means that players will be able to use XP to enchant as much as they want, all they'd need to do is drink something to get 100 XP levels again and gain powerful enchantments.

We recommend that you disable the thirst system if you enable the enchant table.

There are two possible options for `allow_enchants`:

`true|false`

**`drop_exp`**:

Should mobs drop XP orbs?

This defaults to false for the same reason as `allow_enchants`; it will allow players to abuse the fact that they can get an unlimited amount of XP.

Allowing XP orbs to be dropped will also allow players to replenish their thirst without needing to eat or drink.
