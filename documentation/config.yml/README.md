---
description: Learn how to configure UndeadPandemic
cover: >-
  https://images.unsplash.com/photo-1552664730-d307ca884978?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2970&q=80
coverY: 0
---

# config.yml

This is the default config.yml page. The following pages will discuss, in considerable detail, how each configuration section works, and how you can edit the config.yml file to make the plugin do what you want.

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
head_shot_actionBar_Text: '&bYou got a headshot!'
ahow_message_length: 3 # How long the head shot message show appear on screen for, in seconds.

# ENCHANT SETTINGS

allow_enchants: false

# Should mobs drop Exp? It is recommended that this is set to false if you have the thirst system enabled, otherwise the thirst system will not work as intended.

drop_exp: false

# INFECTION SETTINGS

infection:
  
  # enabled by default
  enabled: true
  
  # duration in seconds
  # If empty, or not set, the duration will be 120 seconds.
  duration: 120
  
  # Amplify the effects of the infection. Used in conjunction with the 'amplify_effect' option below.
  amplifier: 10
  
  # Determines whether to amplify all effects of the infection, or just the damage to player.
  # Options: damage_only|all.
  # Option must be surrounded by apostrophes (ex. 'all').
  # If damage_only is set, then all other effects will use the default amplification setting of 10.
  amplify_effect: 'all'

# BARBED WIRE SETTINGS
# Set to -1.0 to disable.
barbed_wire:

  enabled: true
 
  # 1 = half a heart.
  damage: 2

# REWARD SETTINGS

# Currency to award player for killing a zombie.
kill_reward: 10

# Reward if player gets a head shot (will not work when using a shotgun).
kill_reward_head_shot: 15

# Choose to reward player either: instantly when a zombie is killed, or by dropping cash when the zombie is killed
# Use one of these options:
# - instant (default)
# - mobdrop # Only use 'mobdrop' if you are using an item-based economy
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

# Zombies are attracted by the sound of guns. This is how many will spawn within your defined radius whena gun is fired.
# The higher this rate is, the slower your server will be. Be careful with this setting.
attract_zombie_rate: 2

# Attract zombies after a gunshot within this radius of blocks.
attract_zombie_radius: 5

# Chance that a zombie will be attracted by gun fire. chance%
# Set to -1 to disable (this will cause a zombie to be attracted to every gun shot).
attract_zombie_chance: 70

# THIRST SETTINGS

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
  
# KEYCARD SETTINGS

keycard:
  name: 'Key Card'
  lore: 'Opens up doors.'
  material: MUSIC_DISC_STRAD
  data: 123456

# GUN SETTINGS

# If you use other weapons plugins, set this to false.
# This will also disable ammo.
enable_weapons: true

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
