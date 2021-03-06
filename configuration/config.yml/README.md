---
description: Learn how to configure UndeadPandemic
---

# config.yml

This is the default config.yml page. The following pages will discuss, in considerable detail, how each configuration section works, and how you can edit the config.yml file to make the plugin do what you want.

{% hint style="success" %}
The config.yml is a configuration file!
{% endhint %}

## Default config.yml

```
# CORE SETTINGS

# When set to false, players will not require any permissions to use commands or items
require_perms: true

# UndeadPandemic will not function in the worlds listed here.
disable_in_worlds:
#  - 'world'

# MESSAGE SETTINGS

show_message: true # If the headshot message should appear
head_shot_actionbar_text: '&bYou got a headshot!'
show_message_length: 3 # How long the head shot message show appear on screen for, in seconds.

# ENCHANT SETTINGS

allow_enchants: false

# Should mobs drop Exp? It is recommended that this is set to false if you have the thirst system enabled, otherwise the thirst system will not work as intended.

drop_exp: false

# INFECTION SETTINGS

infection:
  
  # enabled by default
  enabled: true
  
  # List of the effects produced by the infection
  # Intensity of the effects can be set by the amplifer option below.
  # Any effect listed by the Spigot API can be used here.
  # Here is the list of effects on the Spigot API
  # https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionEffectType.html
  infection_symptoms:
    - POISON
    - HARM
    - SLOW
    - SLOW_DIGGING
    - HUNGER
    - INCREASE_DAMAGE
    - DAMAGE_RESISTANCE
  
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
  
# ZOMBIE GUTS
  
zombie_guts:
  enabled: true
    
  # Chance
  # Determine the chances that Zombie Guts are dropped as a percentage.
  # Defaults to 3% chance.
  # Chance must be from 1 to 100. If the value is set to less than one or more than 100, then it will default to 3.
  # If you do not want players to have zombie guts, then set 'enabled' to true.
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

  # Set a reward type
  # Types: 'fixed' or 'random'.
  # Reward type defaults to fixed.
  # If set to random, then kill_reward will be ignored. kill_reward_head_shot will also be ignored and will instead default to x1.5 the kill_reward

  reward_type: 'fixed'

  # Reward boundaries
  # Set the minimum and maximum rewards that you'd like the players to receive
  
  min_kill_reward: 5 # defaults to 5
  max_kill_reward: 25 # default to 25

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
  - WITCH
  - WITHER
  - WITHER_SKELETON

# The higher the spawn rate is, the slower your server will be. Be careful with this setting.
# The default is 5, this should be enough to occasionally cause herds.
# Set the spawn rate to -1 to disable it. This will not disable Zombie spawning, it will simply prevent more Zombies from spawning.
# You should restart your server after changing this setting as it may not work when reloading the config.

zombie_spawn_rate: 5

# Zombies are attracted by the sound of guns. This is how many will spawn within your defined radius when a gun is fired.
# The higher this rate is, the slower your server will be. Be careful with this setting.
attract_zombie_rate: 2

# Attract zombies after a gunshot within this radius of blocks.
attract_zombie_radius: 5

# Chance that a zombie will be attracted by gun fire. chance%
attract_zombie_chance: 70

# THIRST SETTINGS

# Set enable_thirst to false to prevent players from gaining XP levels when they use the consumables listed below.
# If enable_thirst is set to true then it is recommended to disable allow_enchants and drop_exp. 
enable_thirst: true
dehydration_rate: 90 # Rate (in seconds) at which thirst will drop by 1%.

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

# HEALTH SETTINGS

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
  
first_aid_kit:
  name: '&4First Aid Kit'
  lore: '&f&oAn emergency first aid kit!'
  data: 2
  
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

# GUN SETTINGS

# If you use other weapons plugins, set this to false.
# This will also disable ammo.
enable_weapons: true

# Should other players be harmed by gun fire? true|false
damage_players: true

# This is how loud the gun fire will be. 1.0 = loudest, 0.0 = silent
gun_fire_volume: 0.5

weapons:
  99p:
    # The type of weapon can be changed to use different ammo.
    type: 'Pistol'
    name: '&fWither 99P'
    lore: '&fAn effective pistol.'
    # Material ID - We used https://www.digminecraft.com/lists/item_id_list_pc.php and recommend that you use it too. Use Minecraft ID NAME (NOT numeric ID). Be careful! You'll have to update the resource pack if you change this option.
    material: MUSIC_DISC_11
    # damage: 20 = 10 Hearts. This should be enough, but you can set it to anything. THIS CANNOT BE ZERO OR NEGATIVE - negative and zero values will default to a damage value of 10
    damage: 20
    # Head shot damage a bonus damage amount that is applied when a player gets head shot. It's recommended that the additional damage is enough to kill the target entity.
    head_shot_damage: 20
    # Clip-size is how many bullets the weapon can hold.
    clip-size: 16
    # Custom model data will allow you to add a texture to the weapon
    custom_model_data: 2
  ak-47:
    type: 'Rifle'
    name: '&fAK-47'
    lore: '&fCheap and effective... sometimes.'
    material: MUSIC_DISC_13
    damage: 20
    head_shot_damage: 20 # Head shot damage is ignored for the AK-47.
    clip-size: 32
    custom_model_data: 2
  barcine:
    type: 'Rifle'
    name: '&fBarcine'
    lore: '&fA powerful semi-automatic rifle.'
    material: MUSIC_DISC_BLOCKS
    damage: 20
    head_shot_damage: 20
    clip-size: 32
    custom_model_data: 2
  mk31:
    type: 'Sniper'
    name: '&fRimmington MK31'
    lore: '&fA military-grade sniper rifle.'
    material: MUSIC_DISC_CAT
    damage: 20
    head_shot_damage: 20
    clip-size: 12
    custom_model_data: 2
  nuck:
    type: 'Shotgun'
    name: '&fNuck Shotgun'
    lore: '&fA shotgun fitting for a farmer, and his mum.'
    material: MUSIC_DISC_CHIRP
    damage: 20
    head_shot_damage: 20
    clip-size: 8
    custom_model_data: 2
  revolver:
    type: 'Revolver'
    name: '&fMagnus Revolver'
    lore: '&fThe classic 6-shot pistol.'
    material: MUSIC_DISC_FAR
    damage: 20
    head_shot_damage: 20
    clip-size: 6
    custom_model_data: 2
    
# AMMO SETTINGS

ammo:
  # ammo type names are case-sensitive
  Pistol:
    name: '&fPistol Bullet'
    lore: '&fBullets for Pistols, obviously.'
    # Custom model data will allow you to add a texture to the ammo.
    # Bullets are modelled from Snowballs.
    custom_model_data: 1
  Revolver:
    name: '&fRevolver Bullet'
    lore: '&fBullets for Revolvers.'
    custom_model_data: 1
  Rifle:
    name: '&fRifle Bullet'
    lore: '&fBullets for rifles and sniper rifles.'
    custom_model_data: 2
  Shotgun:
    name: '&fShotgun Shell'
    lore: '&fShells for a shotguns.'
    custom_model_data: 3
  Sniper:
    name: '&fSniper Bullet'
    lore: '&fMoly-coated.'
    custom_model_data: 2
```
