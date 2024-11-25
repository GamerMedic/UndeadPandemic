# Infected Animals Settings

The Infected Animals system will only affect animals that normally drop food.

**`enabled`**:

This setting will determine if animals are infected or not.

This is set to `true` by default.

**`infection_chance`**:

This is a percentage chance that an animal will be infected.

Set this option to any decimal number between `0.0` and `1.0`. Setting this option to `0.3`, for example, will result in a 30% chance that the water is infected.

If this number is set outside of this range then the plugin will determine the chance for you. You must disable the infected animals system to disable this option.

This option is set to `0.8` by default.

**`animals`**:

You can list which animals can be infected using this option. The default list is below.

```yaml
animals:
  - PIG
  - HOGLIN
  - COW
  - MUSHROOM_COW
  - CHICKEN
  - SHEEP
  - RABBIT
  - SALMON
  - COD
```
