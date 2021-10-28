# Custom Ammunition

You can create custom ammunition by using the config settings used in '[Ammunition Settings](../configuration/config.yml/ammunition-settings.md)'.

For ease, you can copy an paste an existing ammo type and then change as desired.

Here's an example of a custom ammunition type.

```
Flare:
  name: '&4Flare'
  lore: '&e&lNeed help? Fire a flare!'
  custom_model_data: 123456
```

It's that easy.

All ammo types resolve as Snowball projectiles. It's possible to change the texture of the snowball that is fired, but you will have replace the Snowball entirely in the resource pack. Fired projectiles cannot have a custom texture.
