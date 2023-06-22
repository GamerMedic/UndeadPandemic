---
description: >-
  This page details the zombie attributes that can be modified in the config.yml
  file.
---

# 🔢 Zombie Attributes

### Speed

This will determine how quickly the zombies move when attacking the player. The zombie's movement speed when not engaged will remain unaffected.

The vanilla zombie speed value is 0.23. You should set this speed no higher than 1.0, this would guarantee that the zombie catches up with the player. Anything higher can also cause lag.

See the config.yml configuration to see how this value should be set.

If no value is set, then the speed will be set by the plugin.

### Damage

This will determine how much damage zombies deal to others.

The vanilla zombie damage value is 2.0. The default player health is 20.0, so bare this in mind when setting the damage value.

### Health

This will determine the zombies' health.

The vanilla zombie health value is 20.0.

### Knockback Resistance

This will determine the zombies' knockback resistance. Knockback resistance is how much zombies are forced backwards by a players attack and explosions. This can be affected by enchantments to weapons, including bows and arrows.

The vanilla zombie knockback resistance is 0.0. You cannot set this value above 1.0. Setting knockback to 1.0 will guarantee that zombies are not at all affected by attacks or explosions.

### isStupid

This will determine if the zombie will forget that the player is there and will target another entity. This could result in the zombie wondering around confused.

### wearArmour

The `wearArmour` attribute allows you to add armour to zombies, as well as allowing you add enchants to the armour.

You can add the following items: `helmet`, `chestplate`, `leggings`, `boots`.

Add the item and enchants according to the example below.

```
wearArmour:
  helmet: 'LEATHER_HELMET'
  chestplate: 'LEATHER_CHESTPLATE;DURABILITY:3;PROTECTION_FIRE:1'
  leggings: 'LEATHER_LEGGINGS'
  boots: 'LEATHER_BOOTS'
```

`wearArmour` is set to `false` by default, so only include this attribute if you want a zombie to wear armour. You do not have to set a full set of armour. If you only want a zombie to have a helmet, for example, then use the following configuration.

```
wearArmour:
  helmet: 'LEATHER_HELMET'
```

### breakDoors

The `breakDoors` attribute decides whether or not zombies can break doors. This is set to `true` by default.

{% hint style="info" %}
You should only set this attribute if you <mark style="color:red;">**do not**</mark> want the zombie to break doors.
{% endhint %}
