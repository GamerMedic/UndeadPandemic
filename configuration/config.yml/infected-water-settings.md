# Infected Water Settings

**`enabled`**:

Very basic. If this is set to `false` then water will never be infected. Otherwise, there is a chance that the water will be infected when collected from anything other than a filtered cauldron.

This setting is set to `true` by default.

**`purify_water`**:

This setting determines whether the player can purify infected water so that it is drinkable. Pretty mean to set this to `false`, by the way!

This setting is set to `true` by default.

**`infection_chance`**:

This is a percentage chance that water will be infected.

Set this option to any decimal number between `0.0` and `1.0`. Setting this option to `0.3`, for example, will result in a 30% chance that the water is infected.

If this number is set outside of this range then the plugin will determine the chance for you. You must disable the infected water system to disable this option.

This option is set to `0.8` by default.

**`dirty_water_bottle`**:

Use this section to customise the container items. This setting will configure the standard water bottle (potion) when the water inside is infected.

The `dirty_water_bottle` can use the `material`, `name`, `lore`, and `custom_model_data` options.

**`dirty_bucket`**:

This setting will configure the standard water bucket when it contains infected water.

The `dirty_bucket` can use the `name`, `lore`, and `custom_model_data` options.

**`clean_water_bottle`**:

This setting will configure the standard water bottle (potion) when it contains cleaned/purified water.

**`heat_sources`**:

This setting is used to configure a list of valid heat sources for the `filtered_cauldron`. You can use any valid block found on the [spigot list](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html). If you do not want to set any heat sources then set this option as `heat_sources: []`.

If this option is missing from `config.yml` then the plugin will set the following items as heat sources by default.

```yaml
 - MAGMA_BLOCK
 - CAMPFIRE
 - LAVA
```
