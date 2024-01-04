---
description: Learn how to configure UndeadPandemic
---

# 🛠 config.yml

This is the default config.yml page. The following pages will discuss, in considerable detail, how each configuration section works, and how you can edit the config.yml file to make the plugin do what you want.

{% hint style="success" %}
The config.yml is a configuration file!
{% endhint %}

## Default config.yml

```yaml
# CORE SETTINGS

#### DOCUMENTATION: https://docs.stevezr963.me/

# Please do not alter the version number.
# This number identifies the version of the config
# and in future versions this will determine if your config file needs updating.
version: 3

# Set default language
# See the documentation (link above) to find the available languages and the appropriate language code.
# The plugin will default to English
language: 'en'

# When set to false, players will not require any permissions to use commands or items
require_perms: true
# When set to false you will no longer receive an update notification on join.
prompt_on_join: true

# UndeadPandemic will not function in the worlds listed here.
disable_in_worlds: []
#  - 'world_nether'
#  - 'world_end'

## Set this to true if you'd like the worlds blacklist to be treated as a whitelist instead
use_whitelist: false

# The plugin will check for updates in the background and let you know of any updates in the console.
# Set to false if you do not want the plugin to remind you of new updates.
# You will always receive an update check when the plugin is enabled on the server
check_for_updates: true
# If check_for_updates is true, the game will regularly check for new updates.
# This value will tell the plugin how often to check for updates, in hours.
# If this value is less than 1 then it will check for updates every 3 hours by default.
# If this value is set greater than 672 hours (one month) then it will default to 672 hours.
# Set 'check_for_updates' to false to disable this feature.
check_updates_duration: 3

# MESSAGE SETTINGS

show_message: true # If the headshot message should appear
# head_shot_actionbar_text can now be found in the language files.
show_message_length: 3 # How long the head shot message show appear on screen for, in seconds.

# ENCHANT SETTINGS
xp:

  allow_enchants: false
  # Should mobs drop Exp?
  drop_exp: false

# CRAFTING SETTINGS

## List any items that you do not want players to craft.

## Uncomment this line to use a blank list (you must also delete the active list)
#crafting_blacklist: []
crafting_blacklist:
  - LEATHER_HELMET
  - LEATHER_CHESTPLATE
  - LEATHER_LEGGINGS
  - LEATHER_BOOTS
  - IRON_HELMET
  - IRON_CHESTPLATE
  - IRON_LEGGINGS
  - IRON_BOOTS
  - GOLDEN_HELMET
  - GOLDEN_CHESTPLATE
  - GOLDEN_LEGGINGS
  - GOLDEN_BOOTS
  - DIAMOND_HELMET
  - DIAMOND_CHESTPLATE
  - DIAMOND_LEGGINGS
  - DIAMOND_BOOTS
  - CHAINMAIL_HELMET
  - CHAINMAIL_CHESTPLATE
  - CHAINMAIL_LEGGINGS
  - CHAINMAIL_BOOTS
  - NETHERITE_HELMET
  - NETHERITE_CHESTPLATE
  - NETHERITE_LEGGINGS
  - NETHERITE_BOOTS
  - SHIELD

# INFECTION SETTINGS

infection:
  
  # enabled by default
  enabled: true
  
  # Allow new players to be protected from infection
  join_protection:
  
    enabled: true
    # Protection duration (in seconds)
    duration: 180
  
  # Chance of infection
  chance: 40
  
  # List of the effects produced by the infection
  # Intensity of the effects can be set by the amplifer option below.
  # Any effect listed by the Spigot API can be used here.
  # Here is the list of effects on the Spigot API
  # https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionEffectType.html
  
  # Uncomment this line to use a blank list (you must also delete the active list)
  #infection_symptoms: []
  
  infection_symptoms:
    - POISON
    - HARM
    - SLOW
    - SLOW_DIGGING
    - HUNGER
    - DAMAGE_RESISTANCE
    - CONFUSION
  
  # duration in seconds
  # If empty, or not set, the duration will be 120 seconds.
  duration: 120
  
  # Amplify the effects of the infection. Used in conjunction with the 'amplify_effect' option below.
  amplifier: 10
  
  # Determines whether to amplify all effects of the infection, or just the damage to player.
  # Options: damage_only|all.
  # Option must be surrounded by apostrophes (ex. 'all').
  # If damage_only is set, then all other effects will use the default amplification setting of 10.
  # Defaults to all
  amplify_effect: 'all'
  
  # milk cures effects
  # Milk will not cure effects by default
  cure_with_milk: false
  
  # If true, eating Rotten Flesh will infect the player
  infected_rotten_flesh: true
  
# ZOMBIES

# The higher the spawn rate is, the slower your server will be. Be careful with this setting.
# The default is 5, this should be enough to occasionally cause herds.
# Set the spawn rate to -1 to disable it. This will not disable Zombie spawning, it will simply prevent more Zombies from spawning.
# You should restart your server after changing this setting as it may not work when reloading the config.

zombies: # new zombies section.
  
  # Protect villagers from being attacked by zombies
  # (this will stop villagers from taking damage from zombies, but will not stop zombies going after villagers)
  protect_villagers: true
  
  hordes:
    # Increase the rate of the randomly chosen zombie type during a horde.
    # The default setting is 2, which doubles the number of zombies of the chosen type.
    increase_rate: 2
    
  spawn_rate: 2
  # Zombies are attracted by the sound of guns. This is how many will spawn within your defined radius when a gun is fired.
  # The higher this rate is, the slower your server will be. Be careful with this setting.
  attraction_rate: 2
  # Attract zombies after a gunshot within this radius of blocks.
  attraction_radius: 5
  # Chance that a zombie will be attracted by gun fire. chance%
  attraction_chance: 70
  ### Setting this to false will prevent vanilla zombies from spawning so that only custom zombies spawn.
  ### This setting will override to true if enable_custom_zombies = false
  allow_vanilla: true
  # Disable custom zombie spawns
  enable_custom_types: true
  # Disable show_zombie_names to remove the name tags on Zombies.
  show_names: true
  # Disable baby zombies
  allow_babies: true
  # Chance that the stupid zombies will forget that the player is there
  isStupid_chance: 60

zombie_types:
  
  # Vanilla zombie values:
  # speed: 0.23
  # damage: 2.0
  # health: 20.0
  # knockback: 0.0 // This is how resistant zombies are to attacks, explosions, and projectiles. Max is 1.0 (fully resistant)
  
  # 28 Days Later Zombies
  fast:
    enabled: true # Determines if this zombie types appears in the game.
    name: 'Fast Zombie' # Change the name of the zombie.
    spawn_rate: 0.25 # Determines how common zombies are using a weighting.
    speed: 0.75
    damage: 1.0
    health: 20.0
    knockback: 0.0
    canBreakDoors: false # Sets whether this zombie can break doors.
    boss: false # Is this zombie a boss zombie (boss zombies can be recognised as a boss zombie for quests/rewards) || this is a planned feature.
  # Resident Evil Zombies
  strong:
    enabled: true
    name: 'Strong Zombie'
    spawn_rate: 0.1
    speed: 0.25
    damage: 5.0
    health: 50.0
    knockback: 0.7
    canBreakDoors: true
    wearArmour:
      helmet: 'LEATHER_HELMET'
      chestplate: 'LEATHER_CHESTPLATE;DURABILITY:3;PROTECTION_FIRE:1'
      leggings: 'LEATHER_LEGGINGS'
      boots: 'LEATHER_BOOTS'
  # The Walking Dead Zombies
  slow:
    enabled: true
    name: 'Slow Zombie'
    spawn_rate: 2.0
    speed: 0.1
    damage: 2.0
    health: 20.0
    knockback: 0.5
    canBreakDoors: false
  # Shaun of the Dead Zombies
  stupid:
    enabled: true
    name: 'Stupid Zombie'
    spawn_rate: 2.0
    speed: 0.23
    damage: 1.0
    health: 20.0
    knockback: 0.0
    isStupid: true
    breakDoors: false
    canBreakDoors: false

# ZOMBIE GUTS
  
zombie_guts:
  enabled: true
  
  # Customise the zombie guts item and texture
    
  guts:
    name: 'Zombie Guts'
    # A separate 'Use Left' line is added to the lore when dropped by a zombie. This line will contain the guts timer.
    lore:
      - '&4A gross disguise.'
    material: GOLDEN_CHESTPLATE # Don't forget to update your resource pack
    data: 123456 # Custom model data
    
  # Chance
  # Determine the chances that Zombie Guts are dropped as a percentage.
  # Defaults to 3% chance.
  # Chance must be from 1 to 100. If the value is set to less than one or more than 100, then it will default to 3.
  # If you do not want players to have zombie guts, then set 'enabled' to false.
  chance: 3
  
  # Timer
  # How long should zombie effects last, if enabled?
  # If timer is disabled, then the zombie guts will not lose durability over time, except for natural use.
  
  timer:
    # min and max refer to the minimum time and maximum time, in seconds, that the zombie guts should exist while being worn
    min: 5
    max: 120
      
  # fade_in_water determines if the zombie guts should lose durability quicker in water (giving the effect that the water is washing away the smell of the guts)
  # If enabled, then the zombie guts will fade quicker based on the multiplier set below. Default is 2, which means that the zombie guts will lose durability twice as fast as normal.
  # If enabled, zombie guts will break if the player starts to swim
  fade_in_water:
    enabled: true
    multiplier: 2

# BARBED WIRE SETTINGS
# Set to -1.0 to disable.
barbed_wire:

  enabled: true
  # 1 = half a heart.
  damage: 2

# REWARD SETTINGS

# Rewards configured here are given when the player kills a zombie.

rewards:

  enable: true

  # Set a reward type
  # Types: 'fixed' or 'random'.
  # Reward type defaults to fixed.
  # If set to random, then kill_reward will be ignored. kill_reward_head_shot will also be ignored and will instead default to x1.5 the kill_reward

  reward_type: 'fixed'

  # Reward boundaries
  # Set the minimum and maximum rewards that you'd like the players to receive
  
  min_kill_reward: 5 # defaults to 5
  max_kill_reward: 25 # default to 25
  
  multiplier: 1.5

  kill_reward: 10

  # Reward if player gets a head shot (will not work when using a shotgun).
  kill_reward_head_shot: 15

  # Choose to reward player either: instantly when a zombie is killed, or by dropping cash when the zombie is killed
  # Use one of these options:
  # - instant (default)
  # - mobdrop # Only use 'mobdrop' if you are using an item-based economy, or you won't get the reward
  reward_kill: 'instant'

  # Only use these settings if you reward_kill is set to 'mobdrop'.
  # If you don't use an item-based economy, then you can remove the 'reward_item' settings from this config file.

  # Your custom item currency material
  reward_item_material: 'emerald'
  # Your custom item name
  reward_item_name: 'Emerald'
  # Your custom item lore
  reward_item_lore: 'Currency'
  # Your custom item CustomModelData
  reward_item_data: 123456

# MOB SETTINGS

# You can disable any mob by listing it below, or enable disabled mobs by removing them. It is recommended that you add a # to the start of the mob like so:
# - BLAZE
# This will enable the BLAZE mobs and you can disabled them again by removing the #.
# We recommend fetching mob names from https://papermc.io/javadocs/paper/1.16/org/bukkit/entity/package-summary.html
# Do not use numeric IDs, and it's recommended that you use all caps for mob names. Replace all spaces with an underscore ( _ ).
# ZOMBIE will be ignored, because there's no point disabling Zombies in a Zombie Apocalypse plugin :)

# Uncomment this line to use a blank list (you must also delete the active list)
#disable_mobs: []

disable_mobs:
  - BLAZE
  - CAVE_SPIDER
  - CREEPER
  - ENDER_DRAGON
  - ENDERMAN
  - ENDERMITE
  - EVOKER
  - EVOKER_FANGS
  - EVOCATION_ILLAGER
  - EVOCATION_FANGS
  - GHAST
  - GIANT
  - HUSK
  - ILLUSIONER
  - MAGMA_CUBE
  - PHANTOM
  - PILLAGER
  - RAVAGER
  - SKELETON
  - SLIME
  - SPIDER
  - STRAY
  - STRIDER
  - VEX
  - VINDICATOR
  - VINDICATION_ILLAGER
  - WANDERING_TRADER
  - WARDEN
  - WITCH
  - WITHER
  - WITHER_SKELETON
  - ZOGLIN
  - ZOMBIE_VILLAGER

# THIRST SETTINGS

thirst:

  # Disabling thirst will remove the boss bar when players rejoin the server.
  # You will need to restart your server if you change the thirst settings
  enable_thirst: true
  dehydration_rate: 90 # Rate (in seconds) at which thirst will drop by dehydration_qty%.
  dehydration_qty: 5 # as a percentage. Minimum 1%, maxmimum 99%. Just because you CAN set it to 995, doesn't mean you should!
  purify_water: true # Allow water to be purified in a cauldron. Setting this to false will also turn off contaminated water
  disable_bossbar: false # Disable the thirst boss bar. This will prevent the bossbar from loading and will leave the thirst placeholder as the only way to visualise thirst.

  # Set replenishing thirst level for consumables
  consumables:
    APPLE: 2
    BEETROOT_SOUP: 50
    CARROT: 5
    GOLDEN_CARROT: 15
    HONEY_BOTTLE: 15
    MELON_SLICE: 10
    MILK_BUCKET: 75
    MUSHROOM_STEW: 50
    POTION: 75
    RABBIT_STEW: 50
    ROTTEN_FLESH: -15
    SUSPICIOUS_STEW: -10
    WATER_BOTTLE: 75

# INFECTED WATER SETTINGS

infected_water:
  
  enabled: true # When set to false water will never be infected
  purify_water: true # Allow water to be purified in a cauldron. Setting this to false will also turn off contaminated water
  infection_chance: 0.8 # Choose a value between 0.0 and 1.0. This will represent the percentage chance. e.g. 0.3 = 30%
  
  dirty_bucket:
    name: '&5Dirty Water Bucket'
    lore: '&fThis water looks a bit off.'
    custom_model_data: 12345
  
  ## Customise the item when collecting infected water
  dirty_water_bottle:
    material: POTION
    name: '&2Suspicious Water'
    lore: '&4This water looks strange.'
    potion_type: POISON # This is how the potion will look. The default is POISON. A common choice may be WATER
    custom_model_data: 12345
  
  ## Customise the item when collecting clean water
  clean_water_bottle:
    material: POTION
    name: '&bClean Water'
    lore: '&fSafe to drink.'
    potion_type: WATER # This is how the potion will look. The default is POISON. A common choice may be WATER
    custom_model_data: 67890
    
  ##heat_sources: [] ## use this if you want the heat_sources list to be empty
  heat_sources:
    - MAGMA_BLOCK
    - CAMPFIRE
    - LAVA
    
# INFECTED ANIMALS SETTINGS

infected_animals:

  enabled: true # set to false if you do not want animals to drop rotten flesh instead of meat
  infection_chance: 0.8 # A percentage chance that the animal will drop rotten flesh instead. Must be a value between 0.0 and 1.0.
  
  ## Customise name for infected meat
  ## {mob} will be replaced with the name of the mob.
  name: '&2Suspicious {mob} Flesh'
  ## You can remove or add animals that drop meat to this list.
  ## Uncomment the line below and remove the uncommented line to leave the list blank.
  ## infected_animals: []
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
  
# CAMPS

camps:

  # Set default number of chunks given to players on first login
  default_plots: 4
  
  # Set the defaults settings for the safe zone plots.
  set_flags:
  
    # All other WorldGuard region flags that are not listed here will have a default setting, or will be set to make the most realistic world.
    # You can change all other settings by using the worldguard:region commands.
    # Region flags wiki: https://worldguard.enginehub.org/en/latest/regions/flags/#flag-listing
  
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
    interact: false
    # Should players be allowed to use doors or levers, etc?
    use: false
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

# HEALTH SETTINGS

health:

  items:
    adrenaline:
      name: 'Adrenaline'
      lore: 'Temporarily Cure an Infection'
      material: MUSIC_DISC_MALL # Changing the material will require an updated resource pack
      data: 123456

    antibiotics:
      name: 'Antibiotics'
      lore: 'Cure an Infection'
      material: MUSIC_DISC_MELLOHI
      data: 123456

    bandage:
      name: 'Bandage'
      lore: 'Heal Infection Wound'
      material: MUSIC_DISC_STAL
      data: 123456

    paracetamol:
      name: 'Paracetamol'
      lore: 'Take the pain away.'
      material: MUSIC_DISC_CHIRP
      data: 123456
      duration: 60 #in seconds

    codeine:
      name: 'Codeine'
      lore: 'An opioid for the pain.'
      material: MUSIC_DISC_STRAD
      data: 123456
      duration: 120
  
    first_aid_kit:
      ### Player is given a chest with one of all 3 items contained inside
      name: '&4First Aid Kit'
      lore: '&f&oAn emergency first aid kit!'
      data: 2

items:

  # KEYCARD SETTINGS
  keycard:
    name: 'Key Card'
    lore: 'Opens up doors.'
    material: MUSIC_DISC_STRAD
    data: 123456
    # A list of doors that can be opened.
    # This can be set to any valid material, but it'd be silly not to make it a door!
    openable_doors:
      - IRON_DOOR
      - IRON_TRAPDOOR
    
  # TORCH SETTINGS
  torch:
    name: '&fTorch'
    lore: 'Let there be light!'
    material: MUSIC_DISC_WARD
    data: 123456
    duration: 1 # How long a torch will light up an area (in seconds) per unit of battery. Min 1 second. Max 90 seconds.
    
  # BATTERY SETTINGS
  battery:
    name: '&eBattery'
    lore: 'AA. Would probably fit in a torch.'
    material: MUSIC_DISC_WAIT
    data: 123456
  
```
