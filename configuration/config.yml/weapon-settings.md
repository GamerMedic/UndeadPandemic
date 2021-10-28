# Weapon Settings

This is a big section and is used to precisely configure how weapons will look and work within the game.

{% hint style="info" %}
_**TIP**_: It is possible to create your own weapons! See the '[Custom Weapons](../../items/custom-weapons.md)' section for instructions.
{% endhint %}

**`enable_weapons`**:

Should players be able to use weapons in your game?

`true|false`

This setting is best used if you are using another plugin for your weapons.

**`damage_players`**:

Should other players be harmed by gun fire?

`true|false`

**`gun_fire_volume`**:

This is how loud you would like the gun fire to be.

The possible values for this setting are: `0.0 - 1.0`.

`0.0` is silent. `1.0` is the loudest.

{% hint style="warning" %}
This is Minecraft-based setting and cannot be overruled.
{% endhint %}

**`weaponName`**:

This is the ID of the weapon, and how the name of the gun will appear in the tab-complete list when writing the command.

**`type`**:

The type of weapon corresponds to the ammo types. By default, there are 5 valid types:

1. Pistol
2. Revolver
3. Rifle
4. Shotgun
5. Sniper

The type is case-sensitive. If the ammo type has a capital letter, then the `type` setting needs one too.

**`name`**:

This is whatever you want the weapon to be displayed as in-game. Ideally, it will match your weapon's ID name, but it can be whatever your want.

**`lore`**:

Set the lore to anything that you want.

{% hint style="info" %}
_**TIP**_: Minecraft colours can be used in the name and lore.
{% endhint %}

**`material`**:

This is the Minecraft item ID that you'd like to use. For example, `MUSIC_DISC_11`.

**`damage`**:

The `damage` value indicates how much damage will be inflicted to the entity that is shot. The damage value relates to hearts. A value of 1 is half a heart, and 20 is 10 hearts.

This value cannot be lower than 1, and will default to 10 if you set this value to 0 or below.

**`head_shot_damage`**:

This is the same as `damage`, but only applies when the player gets a head shot.

**`clip-size`**:

The `clip-size` is the maximum amount of bullets that can be loaded into the gun at once. This can be set to anything you want.

**`custom_model_data`**:

You can set the custom model data of the weapon to match the item models in your resource pack.
