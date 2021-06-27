# UndeadPandemic

This is a zombie apocalypse plugin made for Spigot 1.16.5.

**LICENCE**: GNU General Public Licence v3.0

### FEATURES

  - Zombies don't die during the day;
  - Zombies form a herd if you stay in one place for too long;
  - Kill instantly with a nicely placed head shot;
  - Customisable kill rewards;
  - Fully customisable weapons, including item material and weapon damage values;
  - Customisable ammunition;
  - Enable/Disable Mobs;
  - Enable/Disable Zombie Exp Drops;
  - Set the Zombie spawn rate;
  - Enable/Disable head shot title message;
  - Barbed wire will cause damage to player;
  - Thirst system.
  - Infection and Cure System
  - Safe Zones

### Install

 1. Download latest files from Spigot or [UndeadPandemic Website](https://undeadpandemic.stevezr963.me).
 2. Unzip folder.
 3. Place UndeadPandemic.jar into plugins folder.
 4. Place UndeadPandemic.zip Resource Pack into resource packs folder.
 5. Restart server.
 6. Set your resource pack to the UndeadPandemic pack.

### Dependencies

The following plugins are **REQUIRED** for UndeadPandemic to work:

  - [Vault](https://www.spigotmc.org/resources/vault.34315/)
  - [WorldEdit](https://dev.bukkit.org/projects/worldedit)
  - [WorldGuard](https://dev.bukkit.org/projects/worldguard)

The following plugins are **RECOMMENDED**; some features may not work without:

  - [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)

### COMMANDS

  *Everyone*:
  
    `/safezone`

  *Admin*:

    `/undeadpandemic <give> <{Player}> <99P|AK-47|Barcine|MK31|Nuck|Revolver|ammo> [if ammo: <Pistol|Rifle|Shotgun>] <{amount}>`
    
    `/undeadpandemicreload | /undeadpandemic reload | /undead reload`
      
### PERMISSIONS

    `undeadpandemic.reload` = Give to OP only by default. Reload the plugin config.yml.
    `undeadpandemic.safezone` = Given to everybody by default. Allows players to create, delete, and modify their safe zones.
    `undeadpandemic.use` = Given to everybody by default. It allows players to interact with the plugin.
    `undeadpandemic.weapons.give` = Given to OP only by default. Allow player to give weapons and ammo to other players (and themselves).
    `undeadpandemic.weapons.use` = Given to everybody by default. Allow player to use weapons and ammo.
    
### PLACEHOLDERS

***(Requires PlaceholderAPI Plugin)***

  "Byter Kills"
    %undeadpandemic_byter_kills% : {placeholderapi_undeadpandemic_byter_kills}
    
  "Head Shots"
    &undeadpandemic_byter_head_shots% : {placeholderapi_undeadpandemic_byter_head_shots}
    
### PLANNED FUTURE FEATURE UPDATES

  - [X] Safe Zones
  - [X] Barbed Wire Player Damage
  - [X] Infection System
  - [ ] First Aid Kits
  - [X] Thirst System
  - [ ] Melee Weapons
  - [X] Weapon & Ammo Sound Bytes
