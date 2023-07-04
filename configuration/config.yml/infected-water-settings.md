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

The `clean_water_bottle` can use the `material`, `name`, `lore`, and `custom_model_data` options.

**`filtered_cauldron`**:

This setting will configure the filtered cauldron item.

The `filter_cauldron` can use the `material`, `name`, `lore`, `custom_model_data`, and `requires_heat` options.

**`options`**:

&#x20;   `material`:

&#x20;       Any valid minecraft material. You can check the [spigot list](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html) to check the proper names.

&#x20;   `name`:

&#x20;       Any name that you like. You can use Minecraft colour codes as normal.

&#x20;   `lore`:

&#x20;       Any description that you like. You can use Minecraft colour codes as normal. This does not yet support multi-line lores.

&#x20;   `customer_model_data`:

&#x20;       Any whole number that you'd like to use. This is only relevant when changing textures.

&#x20;   `potion_type`:

&#x20;       Any potion type that is available from the [spigot API list](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionType.html).

&#x20;       The default type is `POISON`, though `WATER` is a recognised type and may be the universal choice.

&#x20;       `poison_type` only works for the `dirty_water_bottle`.

&#x20;   `requires_heat`:

&#x20;       Determine whether the player needs to place a valid heat source underneath the cauldron. This is set to `true` by default.

&#x20;       Valid heat sources are set in the `heat_sources` setting.

**`heat_sources`**:

This setting is used to configure a list of valid heat sources for the `filtered_cauldron`. You can use any valid block found on the [spigot list](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html). If you do not want to set any heat sources then set this option as `heat_sources: []`.

If this option is missing from `config.yml` then the plugin will set the following items as heat sources by default.

```yaml
Magma Block
Campfire
Lava
```
