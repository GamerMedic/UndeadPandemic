---
description: The default YAML file for the English language.
---

# 🇬🇧 🇬🇧 English

<details>

<summary><code>en.yml</code></summary>

```yaml
messages:
  # Welcome and Premium Messages
  welcome-premium: "Welcome, {playerName}!"
  upgrade-premium: "Upgrade to premium for exclusive benefits!"
  no-premium: "This is a Premium feature!"

  # Player Health and Effects
  thirst-warning: "Warning: Your thirst is low!"
  thirst-buffer: "Your thirst is critically low! You are feeling weak and confused."
  water-purification: "You have purified the dirty water into clean water!"
  analgesia-used: "You have used Analgesia. Your health has been partially restored."
  bandage-used: "You have used a Bandage. Health regeneration has been enabled."
  antibiotics-used: "You have used Antibiotics. All negative effects have been removed."
  adrenaline-used: "You have used Adrenaline. You are now at full health and have damage resistance for 30 seconds."
  infection-applied: "&4You have been infected!"
  
  # Zombie Guts
  zombie-guts-effect-worn-off: "The Zombie Guts effect has worn off."
  zombie-guts-removed-rain: "The Zombie Guts effect has been removed due to the rain."
  zombie-guts-removed-water: "The Zombie Guts effect has been removed due to entering water."
  zombie-guts-created: "*You covered your clothes in the disgusting guts and now you smell rotten!*"
  zombie-guts-chestplate: "I've smeared my top with guts... Gross."
  zombie-guts-status-four: "&4This should last a while."
  zombie-guts-status-three: "&cThis should last long enough."
  zombie-guts-status-two: "&6I won't have long with this."
  zombie-guts-status-one: "&eThis is just a smear, it won't last long at all."
  zombie-guts-status-zero: "&7No point in going anywhere with this."
  zombie-guts-plate-status-four: "&4Fresh and dripping..."
  zombie-guts-plate-status-three: "&cSlick with blood."
  zombie-guts-plate-status-two: "&6Drying. The stench rises."
  zombie-guts-plate-status-one: "&eRotting. Flies gather."
  zombie-guts-plate-status-zero: "&7Falling apart..."

  # Events
  bloodmoon-rises: "&4☾ The Blood Moon Rises... ☾"
  bloodmoon-dawns: "&7☀ The Blood Moon fades as dawn breaks... ☀"
  bloodmoon-dread: "&7A sense of dread fills the air..."

  # Combat and Zombies
  zombie-headshot: "&4&lHeadshot!"
  zombie-bodyshot: "You hit the zombie's body!"

  # Permissions and Restrictions
  no-permission: "You don't have permission to do that."
  players-only-cmd: "Only players can execute this command."
  player-not-found: "Could not find player."
  world-restriction-message: "You cannot use this plugin in the current world: %world%."
  xp-restricted-world: "XP collection is disabled in this world."
  xp-restricted-item: "XP-related items are disabled on this server."

  # Inventory and Crafting
  torch-used: "The torch is now active and provides night vision!"
  torch-out-of-power: "The torch has run out of battery and cannot be used."
  battery-empty: "This battery is empty and cannot be used."
  battery-transferred: "Battery life has been transferred to the torch."
  cannot-switch-during-torch-use: "You cannot switch items while the torch is in use."
  crafting-success: "You have successfully crafted the item!"
  crafting-blacklist: "&4You cannot craft this item!"
  receipe-missing: "The recipe for this item is missing or incomplete."
  invalid-material: "The material for this item is invalid."
  invalid-item: "Invalid item. Available items: Adrenaline, Analgesia, Antibiotics, Bandage, Torch, Battery."
  invalid-qty: "Invalid quantity. Please enter a valid number."

  # Barbed Wire
  no-wire-cutters: "&cYou need wire cutters to remove barbed wire!"
  hurt-by-barbed-wire: "&cYou are hurt by the barbed wire!"

  # Rewards
  reward-money: "You've been rewarded with {amount} coins!"
  reward-items: "You've been rewarded with x{quantity} {itemName}(s)!"

  # Configuration and Updates
  config-reload: "The configuration settings have been reloaded."
  update-plots-err: "&fCould not update {player}'s plot count."

  # Plot Management
  plots-updated: '&2{player} plot count has been adjusted by {new-plots}. They now have {total-plots} plots remaining.'
  missing-plots: '&4Could not fetch your remaining plots.'
  missing-plots-err: '&4You must choose how many plots to give to {player}.'

  # Camp Commands
  camp-cmd-no-player: '&4You must select a player.'
  camp-cmd-no-amount: '&4You must choose how many plots to give to {player}.'
  camp-cmd-no-neg: '&eYou cannot use negative numbers in the /camp command.'
  camp-created: '&eYour camp has been created!'
  camp-created-err: '&4Could not create camp.'
  camp-destroyed: '&eYour camp is no longer safe.'
  camp-destroyed-err: '&cYour camp could not be destroyed.'
  camp-exists: '&ecamp could not be created because one of the same name already exists.'
  camp-info: '------------- &c&l[Camps Info] &r&f-------------'
  camp-info-msg: 'Could not fetch your remaining blocks.'
  camp-plot-count: 'You have &2{plots} &r&fplots left. Use them wisely.'
```

</details>

<details>

<summary>Legacy <code>en.yml(</code>Pre-v3.0.0)</summary>

{% code title="en.yml" overflow="wrap" lineNumbers="true" %}
```yaml
#############################################################
#
#  You can get an updated translation from https://docs.stevezr963.me/getting-started/undeadpandemic/languages/using-translations/english
#
#############################################################
head_shot_actionbar_text: '&bYou got a head shot!'
execution: '&4EXECUTION!'
reload_weapon: '&c&lRELOAD YOUR WEAPON!'
weapon_jammed: '&cYour gun jammed. Try again.'
no_weapon: 'The item you''re holding is not a weapon.'
no_weapon_perms: 'You do not have permission to use weapons.'
getting_thirty: 'You''re getting thirsty!'
thirsty: '&e&lYou''re thirsty'
died_of_thirst: '&7&oYou died of thirst! Dummy.'
dehydrated: '&4&lDEHYDRATION HAS MADE YOU CONFUSED. DRINK SOMETHING, NOW!'
no_door: '&4Door doesn''t exist.'
broken_key: '&eOops! The key card snapped in the lock and is now unusable!'
infected: '&5&lYOU''VE BEEN INFECTED!!!'
no_ammo: '&g&oYou don''t have any bullets to reload.'
no_abx: '&4You are not holding any antibiotics.'
no_adx: '&4You are not holding any adrenaline.'
no_bandage: '&4You are not holding any bandages.'
no_coords: '&4You have not provided full co-ordinates for this keycard.'
no_keycard_uses: '&4The <uses> parameter you set was invalid. Your key card has been created but can only be used once.'
keycard_failed: '&4Could not program key card to open doors.'
sent_ammo_cache: '&2{player} has received their ammunitions cache!'
sent_ammo_cache_error: '&4An ammunitions cache could not be sent.'
received_ammo_cache: '&2You have received an ammunitions cache!'
sent_weapons_cache: '&2{player} has received their weapons cache!'
sent_weapons_cache_error: '&4The weapons cache could not be sent.'
received_weapons_cache: '&2You have received an weapons cache!'
invalid_ammo: 'Invalid ammo type. Valid types: <{ammoTypes}>'
weapons_disabled: '&eWeapons are disabled.'
weapon_not_registered: '&4{weapon} is not a registered weapon. This option is case-sentitive.'
sent_abx: '&2{player} has received their antibiotics (x{amount})!'
sent_abx_err: '&4Antibiotics could not be sent to {player}.'
sent_bandages: '&2{player} has received their bandage(s) (x{amount})!'
sent_bandages_err: '&4Bandage(s) could not be sent to {player}.'
sent_adx: '&2{player} has received their adrenaline (x{amount})!'
sent_adx_err: '&4Adrenaline could not be sent to {player}.'
first_aid_kit_err: '&eCould not create kit.'
invalid_first_aid_kit: '&4{kit} is not a valid item.'
safezone_exists: '&ecamp could not be created because one of the same name already exists.'
invalid_safezone_region: '&4Could not determine existing regions.'
missing_plots: '&4Could not fetch your remaining plots.'
update_plots_err: '&cCould not update plot count. Please notify an admin.'
claimed_plot_err: '&cYou cannot claim foreign land.'
building_safezone: '&eBuilding your camp. Please wait...'
safezone_created: '&eYour camp has been created!'
safezone_created_err: '&4Could not create camp.'
safezone_info: '------------- &c&l[Camps Info] &r&f-------------'
safezone_info_msg: 'Could not fetch your remaining blocks.'
safezone_plot_count: 'You have &2{plots} &r&fplots left. Use them wisely.'
insufficient_plots: '&fYou do not have enough plots to extend your camp.'
destroy_safezone_err: '&5This is not your camp.'
safezone_destroyed: '&eYour camp is no longer safe.'
safezone_destroyed_err: '&cYour camp could not be destroyed.'
wrong_safezone_err: '&5This is not your camp.'
safezone_cmd_no_player: '&4You must select a player.'
safezone_cmd_no_amount: '&4You must choose how many plots to give to {player}.'
safezone_cmd_no_neg: '&eYou cannot use negative numbers in the /camp command.'
cmd_no_console_err: '&4You cannot execute this command from the console.'
cmd_give_param_err: '&4An invalid quantity value was provided in the give command.'
cmd_help_err: '&4Invalid Usage. Usage: /undeadpandemic give <{player}> <ammo|firstaid|torch|weapon> [{amount}]'
player_not_online: '&1{player} is not online.'
cmd_no_perms: '&5You do not have permission to use this command.'
invalid_args: 'Invalid Arguments'
plot_update_err: '&fCould not update {player}''s plot count.'
plots_updated: '&2{player} plot count has been adjusted by {new_plots}. They now have {total_plots} plots remaining.'
invalid_plots: '&4{plots} is not a valid number. You can only use whole numbers here.'
missing_plots_err: '&4You must choose how many plots to give to {player}.'
reload_cmd_success: 'The UndeadPandemic config file has been reloaded.'
invalid_crafting_list: 'Could not build invalid craft list.'
first_aid_kit_inv_err: 'Could not generate first aid kit chest inventory.'
first_aid_no_use: 'Could not use {item}.'
weapons_invalid_list: 'Invalid weapon list.'
guts_no_change: 'Could not change zombie guts data.'
guts_save_err: 'Could not save zombie guts data.'
guts_creation_err: 'Could not create zombie guts.'
guts_drop_err: 'Could not drop zombie guts.'
new_version_msg: '&d&lUPDATE FOUND! Version {new_version} is now available!'
no_update_msg: 'No updates available.'
sent_torch: 'You have sent a torch to {player}!'
sent_torch_err: 'There was a problem delivering the torch.'
received_torch: 'You have received a torch from {player}'
join_protection: '&f* A mist surrounds you *&e You feel stronger and your skin is like stone. This feeling probably won''t last long.'
join_protection_failed: '&4Hey! Don''t let yourself get bitten by a Zombie!'
```
{% endcode %}



</details>
