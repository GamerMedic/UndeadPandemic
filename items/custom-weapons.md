# Custom Weapons

You can create a custom weapon by using the options described in '[Weapon Settings](../configuration/config.yml/weapon-settings.md)'.

For ease, you can simply copy and paste any of the other weapons in the config.yml file and then change the options to match your desired weapon.

Here's an example of a custom weapon (one that doesn't appear in the default config.yml file).

```
beretta:
  type: 'Pistol'
  name: '&e&oBeretta M9'
  lore: '&4A small calibre pistol.'
  material: 'MUSIC_DISC_WAIT'
  damage: 10
  head_shot_damage: 20
  clip_size: 16
  custom_model_data: 123456
```

{% hint style="info" %}
_**TIP**_: You can use a Minecraft ID list to find material names. We used [this one](https://www.digminecraft.com/lists/item\_id\_list\_pc.php).
{% endhint %}

That's it!

This weapon will use the `Pistol` ammo type when firing.
