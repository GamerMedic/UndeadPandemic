# Safe Zone Settings

**`safezone`:**

You can configure how safe zones work using these settings.

`default_plots`**:**

This is the default number of plots that a player can use to build their safe zone. Further plots can be given using the [`/safezone`](../../commands/safezone/) command.

`set_flags`:

You can use this settings to set the default [WorldGuard region flags](https://worldguard.enginehub.org/en/latest/regions/flags/).

Here is the default config.yml set up. This should be self-explanatory, but please ask for help on Discord if you are stuck.

```yaml
# Can players pvp inside safe zones?
pvp: false
# Which mobs, if any, should not be allowed to spawn within the safe zone?
# This option will not allow disabled mobs to spawn
deny_spawn:
  - 'ZOMBIE'
  - 'ZOMBIE_VILLAGER'
# Will TNT explode inside safe zones?
tnt: false
# Can mobs cause damage?
mob_damage: false
# Can players rotate item frames?
rotate_item_frames: false
# Can players destroy item frames?
destory_item_frames: false
# Can players destroy paintings?
destory_painting: false
# LEAVE THIS AS FALSE UNLESS YOU DON'T WANT TO PROTECT THE WORLDGUARD REGION
passthrough: false
# This should be left as false so that only the members of the safe zone can build.
build: false
# Can blocks be mined?
block-break: false
# Can blocks be placed?
block-place: false
# Should players, other than safe zone members, be allowed to use doors, levers, and vehicles?
interact: true
# Should players be allowed to use doors or levers, etc?
use: true
# Can animals be harmed?
damage_animals: true
# Can chests and inventories be accessed?
chest_access: true
# Can vehicles and animals be mounted?
ride: true
# Can players sleep in a bed?
sleep: true
# can respawn anchors be used?
respawn_anchors: true
# Can vehicles be placed?
vehicle_place: true
# Can vehicles be destroyed?
vehicle_destory: true
# Can lighters (flint and steel) be used?
lighter: true
# Can blocks be trampled?
block_trampling: true
# Will frost walker boots work?
frosted_ice_form: true
# Can fireworks cause damage?
firework_damage: true
# Can anvils be used?
use_anvil: true
# Can dripleaves be used?
use_dripleaf: true
# Can pistons be used?
use_pistons: true
```
