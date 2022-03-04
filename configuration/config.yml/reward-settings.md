# Reward Settings

Players can be rewarded for killing zombies.

Reward settings require a vault-based economy. If you do not have Vault _**and**_ an economy plugin which is supported by Vault, such as EssentialsX, then this configuration section will not work.

{% hint style="info" %}
The Reward Settings were updated in v2.4.2.
{% endhint %}

**`reward_type`**:

The `reward_type` option was added in v2.4.2. This option allows you to configure a random reward when the player kills a zombie.

`fixed|random`

The default value for this option is `fixed`. When this value is set to `random`, the `kill_reward` and `kill_reward_head_shot` options will be ignored. Instead, you must use `min_kill_reward` and `max_kill_reward` options.

**`min_kill_reward`**:

This is the minimum kill reward that you wish to give to the player. It is set to 5 by default.

**`max_kill_reward`**:

This is the maximum kill reward that you wish to give to the player. It is set to 25 by default.

**`reward_multiplier`**:

A `reward_multiplier` option will be added in the future. This will allow you to decide on the reward given for a head shot. The `reward_multiplier` was set to 1.5x the given reward by default in v2.4.2.

**`kill_reward`**:

How much currency should the player be rewarded for killing the zombie?

This is set to 10 by default, but you can set this to whatever you want (you shouldn't set this higher than your maximum allowed amount in your economy plugin though).

**`kill_reward_head_shot`**:

This is the same as `kill_reward`, but only applies if the player kills a zombie with a head shot.

**`reward_kill`**:

Should the player be rewarded instantly when they kill the zombie? Or should the zombie drop your custom currency item?

`instant|mob_drop`

This is set to `instant` by default.

If you do use an item-based economy, then you can use the following settings to tell UndeadPandemic what item the zombies should drop.

**`reward_item_material`**:

This is whatever item material names that your custom item uses. Only valid 1.16+ items can be used.

[You can use this site for a list of 1.16 materials](https://minecraftitemids.org).

[You can use this site for a list of 1.17 materials](https://minecraftitemids.com).

You can exlude the "minecraft:" part of the material name.

The default material is 'emerald'.

**`reward_item_name`**:

This is whatever your currency is called. This should be set to the same as the item name you use in your item currency economy plugin.

**`reward_item_lore`**:

Same as `reward_item_name`. It can be whatever you want, but should be the same as in your item currency economy plugin.

**`reward_item_data`**:

If you use custom model data in your economy plugin for your currency, then use that custom model data here.
