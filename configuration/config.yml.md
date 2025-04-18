---
description: Learn how to configure UndeadPandemic
---

# 🛠️ config.yml

This is the default config.yml page. The following pages will discuss, in considerable detail, how each configuration section works, and how you can edit the config.yml file to make the plugin do what you want.

{% tabs %}
{% tab title="Core Settings" %}
`version` The version number for the config file.

{% hint style="warning" %}
Changing the `version` number can result in a corrupted config.yml file.
{% endhint %}

`lang` The default language to be used for in-game messages.

`worlds` Create a blacklist or whitelist of worlds where you want the plugin to work.
{% endtab %}

{% tab title="Premium" %}
`api-key` A special key that is received when a premium licence is purchased.

{% hint style="danger" %}
API keys must be kept secure! Anyone with your key could steal your licence.
{% endhint %}

`api-user` Your Minecraft UUID, used to authenticate you when providing premium features.

{% hint style="info" %}
You can use the [Minecraft UUID Converter](https://mcuuid.net/) to find your UUID if you don't know it. However, it will be supplied with your API key.
{% endhint %}

`api-url` This is the API endpoint where your premium licence is verified.

{% hint style="warning" %}
Do not change this unless instructed to do so by us. We cannot verify your licence from anywhere else.
{% endhint %}
{% endtab %}

{% tab title="Zombies" %}
**`spawn-vanilla-zombies`** Allows vanilla zombies to be turned on or off.

**`custom-zombie-rate`** This is the chance that a custom createdd zombie will be spawned over a vanilla zombie.

**`spawn-rate`** This is the default spawn rate (in seconds) at which zombies will spawn, i.e. 1 zombie will spawn every 5 seconds.

<mark style="color:yellow;">**`sun-burn`**</mark> Determine if zombies are hurt by sunlight. This is `false` by default.

<mark style="color:yellow;">**`see-names`**</mark> Determine if name tags are shown for Zombies. This is `true` by default.

<mark style="color:yellow;">**`spawn-in-daylight`**</mark> Determine if Zombies should spawn during the day.

**`events`** A list of configurable events that add more challenging game play.

**`blood-moon`** Configurable options for the Blood Moon event.

`horde-chance` The percentage chance that a horde will appear during a full moon.

**`types`** A list of different types of zombies.

**`slow`** The name of a type of zombie.

`name` The name for this type of zombie.

`health` The default health for this type of zombie. The higher the health the harder to kill.

`speed` How quickly a zombie can move. `0.2` is the standard walking speed on Minecraft.

`strength` The amount of damage that this type of zombie can inflict in one blow. `2 = 1❤️`

<mark style="color:yellow;">`can-break-doors`</mark> Determines whether or not this type of zombies can break doors down.

`skin` The encoded url skin to make this type of zombie look different from the others.

**`armor`** Options to give armor to this type of zombie. Do not include the `armor` section if you do not want this type of zombie to wear armor.

`helmet` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for a helmet.

`chestplate` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for a chestplate.

`leggings` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for leggings.

`boots` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for boots.

`weapon` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for a weapon, or leave blank for none or default behaviour.

**`drops`** A list of customisable items that may be dropped when a zombie is killed.

`type` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for any item you'd like.

`name` Name of the item dropped.

`lore` Lore of the item dropped. Use multilines to break up the text when required.

`custom-model-data` The CMD ID to provide a custom texture within the texture pack.

`quantity` How many of this item should be dropped each time.

**`infection`** Options for infections from all zombies.

`immunity-duration` How many hours will new users be protected for until they can become infected. Set to `-1` to disable.

`chance` The probability, from 0.0 to 1.0, that the player will be infected when attacked.

**`symptoms`** A list of potion effect buffers that can be modified to suit you.

**`use-milk`** Use milk to cure infections by using the vanilla mechanics. This is disabled by default as otherwise there would be a cure for the infection.

**`guts`** Options for zombie guts

`enabled` Whether or not Zombie Guts will be in the game.

`material` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) to use as guts. Should not be armor or weapons.

`custom-model-data` The CMD ID to provide a texture for the item.

`effective-time-min` The minimum time during which the guts will be effective.

`effective-time-max` The maximum time after which guts will be destroyed.

`effect-duration` How long the zombies will ignore players for.

`slowness-duration` The time, in seconds, that the player will be walking slowly.

`slowness-level` The level of the slowness effect.

`slowness-enabled` Whether or not the player becomes slow while wearing guts.

`lore` The item description.

`weather-removal` Whether or not rain will destroy the guts.

`water-removal` Whether or not swimming in water will destroy the guts.

**`reward`** Set up awards that players will receive upon killing zombies.

`enabled` Determine whether or not players will be rewarded.

`type` Determine what type of reward players will receive, either `money` or an `item`.

`money` If `money`, configure reward.

`amount` How much money players should receive.

`items` If `item`, configure reward.

`type` Provide a [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html).

`quantity` Amount of this item should the player receive.

`name` Give a custom name for this item. If left blank then the vanilla name will be used.

`lore` Give a custom lore for this item. If left blank then the vanilla lore will be used.

**`reward-chance`** A percentage chance that the player will receive a reward when killing a zombie. Set to 100 if they should always receive a reward.
{% endtab %}

{% tab title="Mobs" %}
**`animal-drops`** Configure items dropped by animals when killed.

<mark style="color:yellow;">`enabled`</mark> If set to true then animals that drop food when killed will drop [Rotten Flesh](../items/rotten-flesh.md) instead. Can only be disabled if you have the premium version.

`drop-chance` The likelihood that [Rotten Flesh](../items/rotten-flesh.md) will be dropped, between `0.0` and `1.0`, `1.0` being 100% chance.

**`mobs`** Configure mob spawning.

`use-whitelist` When set to `true` all mob spawning will be disabled. The only mobs that will spawn are zombies and those mobs that are listed in he `whitelist`. If set to `false` then all mobs will spawn as normal.

`whitelist` A list of [valid minecraft mob entities](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/entity/EntityType.html) that will spawn when `use-whitelist` is enabled.
{% endtab %}

{% tab title="Water" %}
**`water`** Configuration settings for water mechanics.

`enabled` If `true` then there is a chance that players will collect dirty water from all water sources.

`dirty-water-chance` The chance that players will collect dirty water instead of normal water when collecting water using a bucket or bottle. Chance between `0.0` and `1.0` where `1.0` is equal to a 100% chance.

**`dirty-bucket`** This is a custom item used in the dirty water mechanics.

`name` Display name for the item.

`lore` Custom lore for the item.

`material` A [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) for the item.

`potion_type` A [valid potion](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionType.html) that will give a different look to the water, as well as an effect of your choosing. The default effect is `POISON`.

`customer_model_data` A CMD ID to give the item a custom texture.

**`heat_sources`** A list of heat sources that will work to purify/boil water. It must be a [valid material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html).
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Thirst" %}
**`thirst`** Configure thirst settings.

`enabled` Determines whether or not the thirst system is active.

`max-thirst` The maximum value for the thirst bar.

`warning-thirst` The level of thirst where players are warned that they are getting thirsty.

`buffer-thirst` The level of thirst where players suffer the effects of thirst through potion effects/buffers.

`dehydration_rate` How quickly, in seconds, the thirst level decreases. This is set to 60 seconds by default. This setting is only available in <mark style="color:yellow;">premium</mark> versions.

`dehydration_amount` How many levels are removed from the thirst bar, this can also be considered a percentage when `max-thirst` is set to 100. This setting is only available in <mark style="color:yellow;">premium</mark> versions.

**`buffers`** Configure the effects enabled when the thirst level hits the `buffer-thirst` threshold.

`effect` Provide a valid [minecraft potion effect](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionEffectType.html).

`duration` How long, in seconds, the effect will last for. The default is `5` seconds.

`amplifier` How powerful the effect will be. The higher the number the more powerful it is. The default is level `1`.

**`display`** Determine how the thirst level should be displayed to the player.

`boss-bar` Allow thirst to be displayed using a boss bar. Or disable the boss bar if it is causing issues.

`placeholder` Allow thirst to be displayed using a placeholder.

**`items`** List of items that can be used to replenish thirst.

`WATER_BOTTLE` A [valid minecraft material](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) name.

`thirst` Amount of thirst that is replenished.

`custom-model-data` The CMD ID of a custom item. Do not include this setting if you are using default items.
{% endtab %}

{% tab title="Experience" %}
**`xp`** Settings for determine how experience points are handled.

`enabled` If set to false then the player cannot collect XP orbs and enchanting will also be disabled.

{% hint style="info" %}
This setting refers to legacy version where thirst was displayed using the XP bar. This is not longer the case and XP can be safely used without affecting any other features.

We still recommend playing with `xp:enabled` set to `false` because it provides a more 'realistic' gameplay scenario.
{% endhint %}
{% endtab %}

{% tab title="Items" %}
**`items`** A list of custom items that are obtainable in the game.

`force-vanilla-overrule` If set to false then only custom items will appear when crafting if you are using a receipe that is the same as the vanilla receipe.

**`analgesia`** Name of custom item.

`name` Give a display name to this item.

`lore` Give a lore to this item.

`custom-model-data` Provide a CMD ID to use a custom texture.

**`crafting-blacklist`** A list of items that cannot be crafted by players. You must use [valid minecraft material names](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html).
{% endtab %}

{% tab title="Camps" %}
`campfires` Settings for campfires.

<mark style="color:yellow;">`douse-in-rain`</mark> When enabled campfires will be doused when it rains.

<mark style="color:yellow;">`interval`</mark> Time in seconds that campfires will be checked again to douse.

<mark style="color:yellow;">`delay`</mark> A switch value that determines if there's a pause after it starts raining before campfires will be doused.

`cauldrons` Settings for cauldrons.

<mark style="color:yellow;">`fill-in-rain`</mark> When enabled cauldrons will fill gradually when it rains.

<mark style="color:yellow;">`interval`</mark> Time in seconds that cauldrons will be checked again to fill.

<mark style="color:yellow;">`delay`</mark> A switch value that determines if there's a pause after it starts raining before cauldrons will start to fill.
{% endtab %}
{% endtabs %}

\*<mark style="color:yellow;">`this-option-is-premium-only`</mark>

<details>

<summary>Complete <code>Config.yml</code> File</summary>

{% code overflow="wrap" lineNumbers="true" %}
```yaml
# CORE SETTINGS
version: 4 # Do not change this number! It is used for compatibility checks.
lang: "en"
worlds:
  # Mode can be either "blacklist" or "whitelist"
  mode: "blacklist"
  
  # List of worlds (world names) to block or allow
  list:
    - world_nether
    - world_the_end

# PREMIUM SETTINGS
premium:
  ## If you have purchased premium then please copy and paste your API key
  ## and UUID here to enable premium features on your server.
  api-key: "YOUR_SECRET_API_KEY"
  api-user: "YOUR_UUID"
  api-url: "https://api.stevezr963.me/"

# ZOMBIE SETTINGS
zombies:
  spawn-vanilla-zombies: true
  custom-zombie-rate: 70 # Percentage chance of custom zombie spawning. This will apply to zombies spawning during the day,
  spawn-rate: 5 # 5 zombies every spawn. This does not apply to zombies spawning during the day.
  spawn-radius: 50 # Within how many blocks will custom zombies spawn?
  sun-burn: false # Set to true if Zombies should be killed in sunlight.
  see-names: true # Set to false if you'd like to have the name tags removed. (Premium)
  spawn-in-daylight: true # Set to false to prevent Zombies spawning in the daylight (Premium).
  sun-burn: false # Set zombies to burn in daylight (Premium)
  pick-up-items: false # Allow zombies to pick up items (Premium)
  body-damage: 0.25 # Premium - Set the amount of damage that hitting the body will inflict. Must be between 0.0 and 1.0 (100%). This is always 0.25 without premium.
  
  # Adjust damage settings
  kills:
    destroy-the-brain: true # Premium - Kills zombies instantly with a single hit to the head. This is always false without premium.
    allow-body-damage: true # Premium - Allow zombies to be killed from hits on any part of the body. This will have no effect if 'destroy-the-brain' is true. This is always true without premium.
    headshot-difficulty: 'normal' # Premium - How easy it should be to get a head shot? Easy|Normal|Hard. Easy may appear to give a head shot on a body hit. This is always 'normal' without premium.
    
  
  # Events are premium
  events:
    blood-moon:
      horde-chance: 50

  types:
    slow:
      name: "Slow Zombie"
      health: 30.0
      speed: 0.1
      strength: 2
      can-break-doors: false
      skin: "default"
      armor:
        helmet: "IRON_HELMET"
        chestplate: "IRON_CHESTPLATE"
        leggings: "IRON_LEGGINGS"
        boots: "IRON_BOOTS"
      weapon: "WOODEN_SWORD"
    
    strong:
      name: "Strong Zombie"
      health: 80.0
      speed: 0.2
      strength: 8
      can-break-doors: true
      skin: "default"
      armor:
        helmet: "DIAMOND_HELMET"
        chestplate: "DIAMOND_CHESTPLATE"
        leggings: "DIAMOND_LEGGINGS"
        boots: "DIAMOND_BOOTS"
      weapon: "DIAMOND_SWORD"

    stupid:
      name: "Stupid Zombie"
      health: 50.0
      speed: 0.05
      strength: 1
      can-break-doors: false
      skin: "default"
      armor:
        helmet: "LEATHER_HELMET"
        chestplate: "LEATHER_CHESTPLATE"
        leggings: "LEATHER_LEGGINGS"
        boots: "LEATHER_BOOTS"
      weapon: "STICK"

    default:
      name: "" # Leave empty if you don't want to see a name tag for vanilla zombies
      health: 40.0
      speed: 0.3
      strength: 5
      can-break-doors: true
      skin: "default"
      armor:
        helmet: "CHAINMAIL_HELMET"
        chestplate: "CHAINMAIL_CHESTPLATE"
        leggings: "CHAINMAIL_LEGGINGS"
        boots: "CHAINMAIL_BOOTS"
      weapon: "IRON_SWORD"

  # Custom drops for zombies
  disable-drops: false # When set to true zombies will not drop any items unless reward.type is 'item'.
  drops:
    - type: "ROTTEN_FLESH" # Item type
      name: "Zombie Flesh" # Display name
      lore: # Item lore
        - "Eww, it's from a zombie!"
        - "Will you eat it?"
      custom-model-data: 12345 # Custom model data
      quantity: 5 # Amount to drop
    - type: "IRON_INGOT"
      name: "Shiny Iron"
      lore:
        - "A piece of iron, pure and shiny."
        - "Can be used for crafting."
      custom-model-data: 67890
      quantity: 1

  # INFECTION SETTINGS
  infection:
    immunity-duration: 3 # Immunity period in hours (on first login)
    # Probability of infection upon zombie attack (0.0 to 1.0)
    chance: 0.5

    # Effects of the infection on players
    # Format: EFFECT_NAME:DURATION_IN_SECONDS:AMPLIFIER
    symptoms:
      - POISON:10:1
      - SLOW:20:2
      - WEAKNESS:15:1
      - HUNGER:30:1
      
    use-milk: false # If set to true players will be able to use the vanilla action of milk to remove infection buffers.
      
  # GUTS SETTINGS
  guts:
    enabled: true                   # Enable or disable the Zombie Guts feature
    material: SLIME_BLOCK           # The material used for the Zombie Guts item
    custom-model-data: 12345        # The custom model data for the item
    effect-time-min: 30             # The minimum amount of time (in seconds) that the guts will survive
    effect-time-max: 120            # The maximum amount of time (in seconds) that the guts will survive
    effect-duration: 120            # How long the zombies ignore the player (in seconds)
    slowness-duration: 60           # Duration for the slowness effect (in seconds)
    slowness-level: 1               # Level of the slowness effect (0 = No effect, 1 = Slowness I, etc.)
    slowness-enabled: true          # Whether to apply the slowness effect or not
    name: "&6Zombie Guts"
    lore:
      - "&7Worn to mask your scent"
      - "&7Zombies will ignore you for a while"
    weather-removal: true           # Remove Zombie Guts effect if it rains
    water-removal: true             # Remove Zombie Guts effect if the player enters water
      
  # REWARD SETTINGS
  reward:
    enabled: true  # Enable or disable rewards
    type: "money"  # Can be either "money" or "item"
  
    # Money reward settings
    money:
      amount: 100  # Amount of money to reward

    # Item reward settings
    items:
      - type: "DIAMOND"
        quantity: 1
        name: "Shiny Diamond"
        lore:
          - "A precious gem."

    # Optional chance to reward either money or items
    reward-chance: 50  # Percentage chance to reward money (0-100)
    
# ANIMAL DROP SETTINGS
animal-drops:
  enabled: true  # Enable/disable animal mobs dropping rotten flesh
  drop-chance: 0.75  # Chance of dropping rotten flesh (0.0 to 1.0)
  
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
  
mobs:
  # Passive mobs are not affected.
  use-whitelist: true # When enabled, mob spawning will be disabled for all mobs except zombies and those listed on the whitelist.
  whitelist: # Only those mobs listed here will spawn (except zombies which will always spawn).
    - ZOMBIE_VILLAGER
  
# Water collection settings
water:
  enabled: true
  dirty-water-chance: 0.75 # 50% chance to collect dirty water when filling a bucket or bottle # Premium
  
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
  
# THIRST SETTINGS
thirst:
  enabled: true                 # Enable or disable thirst system
  max-thirst: 100               # Maximum thirst level
  warning-thirst: 30            # Thirst level to trigger hotbar warning
  buffer-thirst: 10             # Thirst level to trigger confusion and weakness effects
  dehydration_rate: 60          # How quickly thirst will decrease in seconds. (PREMIUM)
  dehydration_amount: 5         # By what percentage thirst will decrease, i.e. decrease 5% every 60 seconds. (PREMIUM)
  buffers:
    - effect: "CONFUSION"   # Effect to apply
      duration: 200          # Duration in ticks (10 seconds)
      amplifier: 1           # Effect level (1 = level 2)
    - effect: "WEAKNESS"
      duration: 200
      amplifier: 1
  display:
    boss-bar: true              # Show thirst as a boss bar
    placeholder: true           # Use PlaceholderAPI for thirst display

  items:
    POTION:                     # Water bottle
      thirst: 20                # Amount of thirst replenished
      #custom-model-data: 1      # Custom model data for the item

    SWEET_BERRIES:
      thirst: 10
      #custom-model-data: 2

    MELON_SLICE:
      thirst: 15
      #custom-model-data: 3

    MILK:
      thirst: 20
      #custom-model-data: 3
      
xp:
  enabled: false

items:
  # Option to force vanilla items to override custom items with the same recipe
  force-vanilla-override: true  # Set to false if you want custom items to take precedence
  analgesia:
    name: "Analgesia"
    lore:
      - "Stops pain and restores some health."
    custom-model-data: 1
    recipe: "analgesia"
  bandage:
    name: "Bandage"
    material: "MUSIC_DISC_13"
    lore:
      - "Regenerates health over time"
    custom-model-data: 2
    recipe: "bandage"
  antibiotics:
    name: "Antibiotics"
    material: "MUSIC_DISC_13"
    lore:
      - "Removes all negative effects"
    custom-model-data: 3
    recipe: "antibiotics"
  adrenaline:
    name: "Adrenaline"
    material: "MUSIC_DISC_13"
    lore:
      - "Keeps you at full health for a while"
    custom-model-data: 4
    recipe: "adrenaline"
  torch:
    name: "Torch"
    material: "BLAZE_ROD"
    lore:
      - "A source of light in the dark."
      - "Charge: %charge%%"
    custom-model-data: 5
    recipe: "torch"
  battery:
    name: "Battery"
    material: "REDSTONE"
    lore:
      - "Powers your torch."
      - "Charge: %charge%%"
    custom-model-data: 6
    max-life: 100  # Max battery life for the battery
    recipe: "battery"
  barbed-wire:
    name: "Barbed Wire"
    lore:
      - "A dangerous trap."
      - "Hurts anyone who moves through it."
    custom-model-data: 12345
    ## /************** hurts-mobs ****************
    ## ** Can only be enabled using premium.
    ## ** Be careful using this as it may cause lag.
    ## ** Lag should be minimal, but if you experience lag then you can either reduce the zombie or mob spawn rates,
    ## ** or disable this feature.
    ## ******************************************/
    hurts-mobs: false
    recipe: "barbed-wire"
  wire-cutters:
    name: "Wire Cutters"
    lore:
      - "Essential tool for removing barbed wire."
      - "Only available to premium players."
    custom-model-data: 54321
    recipe: "wire-cutters"
    
  crafting-blacklist:
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

camps:
  campfires:
    douse-in-rain: true # Premium - When enabled camp fires will be doused when it rains. This requires a server restart.
    interval: 25 # Checks for re-lit fires every n seconds.
    delay: true # delays the check by the interval. When set to 'false' the check will happen instantly.
  cauldrons:
    fill-in-rain: true # Premium - When enabled caulrons will be filled with rain water. This requires a server restart.
    interval: 25 # Fills by one level every n seconds.
    delay: true
```
{% endcode %}



</details>
