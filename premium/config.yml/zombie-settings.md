# Zombie Settings

Zombie settings determine chance of zombies spawning, as well the rate that they spawn, and whether zombies are attracted by gun fire.

**`zombie_spawn_rate`**:

The rate at which zombies will spawn during the night. This is set to `5` by default. This can be any integer.

Disable the spawn rate by setting this value to `-1`. Disabling the spawn right doesn't prevent zombies from spawning, it only restricts the zombie spawn rates to the vanilla settings.

{% hint style="danger" %}
The higher that the spawn rate is the slower that your server will be. So unless you have a supercomputer as your Minecraft server, do not set this rate above 10.
{% endhint %}

**`attract_zombie_rate`**:

This rate will determine how many zombies spawn when a loud weapon is used. This defaults to `2`. Same rules apply as the **`zombie_spawn_rate`**; don't set this rate above 10.

**`attract_zombie_radius`**:

This radius will determine how far away (in blocks) zombies will spawn when a loud weapon is used.

This defaults to `5` but for realism it is recommended to set this to at least `7`. Just bear in mind that the higher the radius, the higher the CPU load, especially when combined with a higher **`attract_zombie_rate`**.

**`attract_zombie_chance`**:

This is the percentage chance that zombies will be attracted to the sound of loud weapons. This is set to `70%` by default. This setting must be between 0 and 100, you can set it as any number but the plugin will ignore the abnormal setting. Instead, if this is set above 100 then the chance will be set to 100%, and below 0 the chance will be set to 0%.

**`zombie_types`**:

You can enable and disable zombie types in this section, as well as set the odds of each zombie type spawning.

You can create a new type of zombie by using the configuration attributes below. Vanilla zombies are enabled by default, so if there are no types set then vanilla zombies will still be enabled.

{% hint style="info" %}
You cannot change the settings for vanilla zombies. They will automatically have a weighting of 25.0. They will still result in a 100% chance if no other types exist.
{% endhint %}

**`isStupid_chance`**:

Set the chance that stupid zombies will forget that the player is there. Default is 60.

**`enabled`**:

Use this setting to determine if the parent type should appear in the game.

`values`: `true | false`

**`spawn_rate`**:

The `spawn_rate` in the `zombie_types` section is used to determine the odds of a zombie of the parent type spawning near the player. The spawn rate uses a weighting, this means that the higher the weighting the more likely that type is to spawn. However, if weightings are close together, for example, using weightings of 20.0 and 25.0, then there will be little difference in the chances of spawning that type.

Weightings do not have to add up to 100 as they are not percentage values.

All zombie type spawn rates are set to 25.0 by default.

**`speed`**`:`

Set the zombies' speed using this value.

`Values: 0.1 - 1.0`

An out of range value will cause the speed to default to 0.2.

**`damage`**:

Set the zombies' damage value.

The default value is 2.0

`Minimum value: 0.1`

**`health`**:

Set the zombies' health.

The minimum allowed value is 1.0 (one half a heart).

**`knockback`**:

Set the zombie knockback resistance. You cannot set this value outside of the stated value range below. If you try to set this value outside of the range then the plugin will change the value.

`Values: 0.0 - 1.0`

**`canBreakDoors`**:

When set to `true` the zombie will be able to break down doors.

`Values: true|false`

**`isStupid`**`:`

Determine is the zombie is stupid (forgets that the player is there and targets another nearby entity instead.

`false by default`

See '[Zombie Attributes](../../systems/zombies/zombie-attributes.md)' for more information.

### Create New Zombie

Create a type name for your new zombie in the `zombie_types` section of the config.yml file, and then add each of the attributes you'd like to change. Using the `enabled` setting is optional. If any zombies are built in the `zombie_types` section then they will be enabled by default.

#### Example

```
isStupid_chance: 30
newZombie:
  name: '&4Super Zombie'
  spawn_rate: 25.0
  speed: 0.1
  damage: 5.0
  health: 40.0
  knockback: 0.5
  isStupid: false
```
