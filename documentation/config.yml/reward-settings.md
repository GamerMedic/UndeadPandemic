# Reward Settings

Players can be rewarded for killing zombies.

Reward settings require a vault-based economy. If you do not have Vault _**and **_an economy plugin which is supported by Vault, such as EssentialsX, then this configuration section will not work.

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
