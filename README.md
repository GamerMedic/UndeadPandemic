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
  - Enable/Disable head shot title message.
  - Barbed wire will cause damage to player.

### COMMANDS

  *Root*:
  
    /undeadpandemic | /undead

  *Admin*:

    /undeadpandemic <give> <{Player}> <99P|AK-47|Barcine|MK31|Nuck|Revolver|ammo> [if ammo: <Pistol|Rifle|Shotgun>] <{amount}>
    
    /undeadpandemicreload | /undeadpandemic reload | /undead reload
    
  ***Command Explanation***
  
  <*Required*>
  
  [*Optional*]
  
  {Player} = The name of the player that you would like to give the item to. The player must be online.
  
  <99P|AK047|Barcine|MK31|Nuck|Revolver> = Weapon names.
  
  <|ammo> = Give the player ammo.
  
  [if ammo:] = If you are giving the player ammo use <Pistol|Rifle>, otherwise, ignore.
  
  <Pistol|Rifle|Shotgun> = Weapon types. These also indicate the required ammo. You can use Pistol ammo with a rifle, etc. This is case-sensitive and so will not work with lower case first characters.
    
  {amount} = The amount that you want to give.
    
##### Command Examples

    Give a gun and ammo to SteveZR963:
    
      /undead give stevezr963 99P 1
      
      /undead give stevezr963 ammo Pistol 10
      
### PERMISSIONS

    undeadpandemic.use = Given to everybody by default. It allows players to interact with the plugin.
    undeadpandemic.weapons.give = Given to OP only by default. Allow player to give weapons and ammo to other players (and themselves).
    undeadpandemic.weapons.use = Given to everybody by default. Allow player to use weapons and ammo.
    undeadpandemic.reload = Give to OP only by default. Reload the plugin config.yml.
    
### PLACEHOLDER API

  "Byter Kills"
    %undeadpandemic_byter_kills% : {placeholderapi_undeadpandemic_byter_kills}
    
  "Head Shots"
    &undeadpandemic_byter_head_shots% : {placeholderapi_undeadpandemic_byter_head_shots}
    
### PLANNED FUTURE FEATURE UPDATES

  - [ ] Safe Zones & Camps
  - [X] Barbed Wire Player Damage
  - [ ] Infection System
  - [ ] First Aid Kits
  - [ ] Thirst System
  - [ ] Melee Weapons
  - [ ] Weapon & Ammo Sound Bytes
