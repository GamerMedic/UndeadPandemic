---
description: >-
  Het standaard YAML-bestand voor de Nederlandse taal. (Aangeboden door Google
  Translate)
---

# 🇳🇱 🇳🇱 Nederlands

<details>

<summary><code>nl.yml</code></summary>

```yaml
messages:
  # Welcome and Premium Messages
  welcome-premium: "Welkom, {playerName}!"
  upgrade-premium: "Upgrade naar premium voor exclusieve voordelen!"
  no-premium: "Dit is een premium functie!"

  # Player Health and Effects
  thirst-warning: "Waarschuwing: Je dorst is laag!"
  thirst-buffer: "Je dorst is kritiek laag! Je voelt je zwak en verward."
  water-purification: "Je hebt het vuile water gezuiverd naar schoon water!"
  analgesia-used: "Je hebt Analgesia gebruikt. Je gezondheid is gedeeltelijk hersteld."
  bandage-used: "Je hebt een Verband gebruikt. Gezondheidsregeneratie is ingeschakeld."
  antibiotics-used: "Je hebt Antibiotica gebruikt. Alle negatieve effecten zijn verwijderd!"
  adrenaline-used: "Je hebt Adrenaline gebruikt. Je bent nu volledig gezond en hebt 30 seconden schadebestendigheid."
  infection-applied: "&4Je bent geïnfecteerd!"

  # Zombie Guts
  zombie-guts-effect-worn-off: "Het effect van de Zombie Guts is verdwenen."
  zombie-guts-removed-rain: "Het effect van de Zombie Guts is verwijderd door de regen."
  zombie-guts-removed-water: "Het effect van de Zombie Guts is verwijderd door het betreden van water."
  zombie-guts-created: "*Je hebt jezelf bedekt met die walgelijke ingewanden en nu stink je naar rotting!*"
  zombie-guts-chestplate: "Ik heb mijn bovenkleding besmeurd met ingewanden... Bah."
  zombie-guts-status-four: "&4Dit zou een tijdje moeten duren."
  zombie-guts-status-three: "&cDit zou genoeg moeten duren."
  zombie-guts-status-two: "&6Ik heb niet veel tijd meer met dit."
  zombie-guts-status-one: "&eDit is slechts een vlek, het duurt niet lang."
  zombie-guts-status-zero: "&7Dit heeft geen zin, je kunt hier niet verder mee."
  zombie-guts-plate-status-four: "&4Vers en druipend..."
  zombie-guts-plate-status-three: "&cGlad van bloed."
  zombie-guts-plate-status-two: "&6Aan het opdrogen. De geur wordt sterker."
  zombie-guts-plate-status-one: "&eIn ontbinding. Vliegen verzamelen zich."
  zombie-guts-plate-status-zero: "&7Het valt uit elkaar..."

  # Events
  bloodmoon-rises: "&4☾ De Bloedmaan stijgt... ☾"
  bloodmoon-dawns: "&7☀ De Bloedmaan verdwijnt bij het ochtendgloren... ☀"
  bloodmoon-dread: "&7Een gevoel van angst vult de lucht..."

  # Combat and Zombies
  zombie-headshot: "&4&lHoofdschot!"
  zombie-bodyshot: "Je hebt het lichaam van de zombie geraakt!"

  # Permissions and Restrictions
  no-permission: "Je hebt geen toestemming om dit te doen."
  players-only-cmd: "Alleen spelers kunnen deze commando uitvoeren."
  player-not-found: "Speler niet gevonden."
  world-restriction-message: "Je kunt deze plugin niet gebruiken in de huidige wereld: %world%."
  xp-restricted-world: "XP verzamelen is uitgeschakeld in deze wereld."
  xp-restricted-item: "XP-gerelateerde items zijn uitgeschakeld op deze server."

  # Inventory and Crafting
  torch-used: "De fakkel is nu actief en biedt nachtzicht!"
  torch-out-of-power: "De fakkel is zonder stroom en kan niet gebruikt worden."
  battery-empty: "Deze batterij is leeg en kan niet gebruikt worden."
  battery-transferred: "De batterij is overgedragen naar de fakkel."
  cannot-switch-during-torch-use: "Je kunt geen items wisselen terwijl de fakkel in gebruik is."
  crafting-success: "Je hebt het item succesvol gecreëerd!"
  crafting-blacklist: "&4Je kunt dit item niet maken!"
  receipe-missing: "Het recept voor dit item ontbreekt of is incompleet."
  invalid-material: "Het materiaal voor dit item is ongeldig."
  invalid-item: "Ongeldig item. Beschikbare items: Adrenaline, Analgesia, Antibiotica, Verband, Fakkel, Batterij."
  invalid-qty: "Ongeldige hoeveelheid. Voer een geldig nummer in."

  # Barbed Wire
  no-wire-cutters: "&cJe hebt draadknippers nodig om het prikkeldraad te verwijderen!"
  hurt-by-barbed-wire: "&cJe bent gewond door het prikkeldraad!"

  # Rewards
  reward-money: "Je bent beloond met {amount} munten!"
  reward-items: "Je bent beloond met x{quantity} {itemName}(s)!"

  # Configuration and Updates
  config-reload: "De configuratie-instellingen zijn opnieuw geladen."
  update-plots-err: "&fKon het aantal percelen van {player} niet bijwerken."

  # Plot Management
  plots-updated: '&2Het aantal percelen van {player} is aangepast met {new-plots}. Ze hebben nu {total-plots} percelen over.'
  missing-plots: '&4Kon het resterende aantal percelen niet ophalen.'
  missing-plots-err: '&4Je moet kiezen hoeveel percelen je aan {player} wilt geven.'

  # Camp Commands
  camp-cmd-no-player: '&4Je moet een speler selecteren.'
  camp-cmd-no-amount: '&4Je moet kiezen hoeveel percelen je aan {player} wilt geven.'
  camp-cmd-no-neg: '&eJe kunt geen negatieve getallen gebruiken in de /camp-commando.'
  camp-created: '&eJe kamp is aangemaakt!'
  camp-created-err: '&4Het kamp kon niet worden aangemaakt.'
  camp-destroyed: '&eJe kamp is niet meer veilig.'
  camp-destroyed-err: '&cJe kamp kon niet worden vernietigd.'
  camp-exists: '&eHet kamp kon niet worden aangemaakt omdat er al een kamp met die naam bestaat.'
  camp-info: '------------- &c&l[Informatie over Kampen] &r&f-------------'
  camp-info-msg: 'Kon het resterende aantal blokken niet ophalen.'
  camp-plot-count: 'Je hebt &2{plots} &r&fpercelen over. Gebruik ze verstandig.'
```

</details>

<details>

<summary>Legacy <code>nl.yml</code> (Pre-v3.0.0)</summary>

{% code title="nl.yml" overflow="wrap" lineNumbers="true" %}
```yaml
#############################################################
#
#  U kunt een bijgewerkte vertaling krijgen van https://docs.stevezr963.me/getting-started/undeadpandemic/languages/using-translations/nederlands
#
#############################################################

head_shot_actionbar_text: '&bJe hebt een hoofdschot!'
execution: '&4EXECUTIE!'
reload_weapon: '&c&lHERLAAD JE WAPEN!'
weapon_jammed: '&cJe wapen is vastgelopen. Probeer het nog eens.'
no_weapon: 'Het item dat je vasthoudt is geen wapen.'
no_weapon_perms: 'Je hebt geen toestemming om wapens te gebruiken.'
getting_thirty: 'Je krijgt dorst!'
thirsty: '&e&lJe hebt dorst'
died_of_thirst: '&7&oJe stierf van de dorst! Idioot.'
dehydrated: '&4&lDEHYDRATIE HEEFT U IN DE VERWARRING GEHAD. DRINK IETS, NU!'
no_door: '&4Deur bestaat niet.'
broken_key: '&eOeps! De sleutelkaart is in het slot geknapt en is nu onbruikbaar!'
infected: '&5&lJE BENT GENFECTEERD DOOR EEN ZOMBIE!!!'
no_ammo: '&g&oJe hebt geen kogels om te herladen.'
no_abx: '&4Je hebt geen antibiotica in je hand.'
no_adx: '&4Je houdt geen adrenaline vast.'
no_bandage: '&4U houdt geen verband vast.'
no_coords: '&4U heeft geen volledige coördinaten voor deze keycard opgegeven.'
no_keycard_uses: '&4De parameter <uses> die u heeft ingesteld, is ongeldig. Uw keycard is aangemaakt, maar kan maar één keer worden gebruikt.'
keycard_failed: '&4Kan de sleutelkaart niet programmeren om deuren te openen.'
sent_ammo_cache: '&2{player} heeft hun munitiecache ontvangen!'
sent_ammo_cache_error: '&4Een munitiecache kon niet worden verzonden.'
received_ammo_cache: '&2Je hebt een munitiecache ontvangen!'
sent_weapons_cache: '&2{player} heeft hun wapencache ontvangen!'
sent_weapons_cache_error: '&4De wapencache kon niet worden verzonden.'
received_weapons_cache: '&2Je hebt een wapencache ontvangen!'
invalid_ammo: 'Ongeldig soort munitie. Geldige typen: <{ammoTypes}>'
weapons_disabled: '&eWapens zijn uitgeschakeld.'
weapon_not_registered: '&4{weapon} is geen geregistreerd wapen. Deze optie is hoofdlettergevoelig.'
sent_abx: '&2{player} hun antibiotica heeft gekregen (x{amount})!'
sent_abx_err: '&4Er kon geen antibiotica worden opgestuurd naar {player}.'
sent_bandages: '&2{player} hun verband(len) heeft ontvangen (x{amount})!'
sent_bandages_err: '&4Verband(en) konden niet worden verzonden naar {player}.'
sent_adx: '&2{player} heeft hun adrenaline gekregen (x{amount})!'
sent_adx_err: '&4Adrenaline kon niet verzonden worden naar {player}.'
first_aid_kit_err: '&eKon de kit niet maken.'
invalid_first_aid_kit: '&4{kit} is geen geldig artikel.'
safezone_exists: '&eVeilige zone kan niet worden gemaakt omdat er al een met dezelfde naam bestaat.'
invalid_safezone_region: '&4Kan bestaande regio''s niet bepalen.'
missing_plots: '&4Kan uw resterende plots niet ophalen.'
update_plots_err: '&cKan plottelling niet bijwerken. Breng een beheerder op de hoogte.'
claimed_plot_err: '&cU kunt geen aanspraak maken op buitenlands land.'
building_safezone: '&eBouwen aan je veilige zone. Even geduld aub...'
safezone_created: '&eJe veilige zone is gecreëerd!'
safezone_created_err: '&4Kan veilige zone niet maken.'
safezone_info: '------------- &c&l[Informatie over veilige zones] &r&f-------------'
safezone_info_msg: 'Kan uw resterende blokken niet ophalen.'
safezone_plot_count: 'Je hebt &2{plots} &r&fplots over. Gebruik ze verstandig.'
insufficient_plots: '&fJe hebt niet genoeg percelen om je veilige zone uit te breiden.'
destroy_safezone_err: '&5Dit is niet je veilige zone.'
safezone_destroyed: '&eJe veilige zone is niet langer veilig.'
safezone_destroyed_err: '&cJe veilige zone kon niet worden vernietigd.'
wrong_safezone_err: '&5Dit is niet je veilige zone.'
safezone_cmd_no_player: '&4Je moet een speler selecteren.'
safezone_cmd_no_amount: '&4Je moet kiezen hoeveel plots je aan {player} wilt geven.'
safezone_cmd_no_neg: '&eU kunt geen negatieve getallen gebruiken in het /safezone-commando.'
cmd_no_console_err: '&4U kunt deze opdracht niet uitvoeren vanaf de console.'
cmd_give_param_err: '&4Er is een ongeldige hoeveelheidswaarde opgegeven in de opdracht give.'
cmd_help_err: '&4Ongeldig gebruik. Gebruik: /undeadpandemic give <{player}> <ammo|firstaid|torch|weapon> [{amount}]'
player_not_online: '&1{player} is niet online.'
cmd_no_perms: '&5U heeft geen toestemming om deze opdracht te gebruiken.'
invalid_args: 'Ongeldige argumenten'
plot_update_err: '&fKan de plottelling van {player} niet updaten.'
plots_updated: '&2Het aantal plotnummers van {player} is aangepast door {new_plots}. Ze hebben nu nog {total_plots} percelen over.'
invalid_plots: '&4{plots} is geen geldig nummer. U kunt hier alleen hele getallen gebruiken.'
missing_plots_err: '&4Je moet kiezen hoeveel plots je aan {player} wilt geven.'
reload_cmd_success: 'Het UndeadPandemic-configuratiebestand is opnieuw geladen.'
invalid_crafting_list: 'Kan geen ambachtelijke lijst maken omdat deze ongeldig is.'
first_aid_kit_inv_err: 'Kan de inventaris van de EHBO-kist niet genereren.'
first_aid_no_use: 'Kan {item} niet gebruiken.'
weapons_invalid_list: 'Ongeldige wapenlijst.'
guts_no_change: 'Kan gegevens over zombie-lef niet wijzigen.'
guts_save_err: 'Kon gegevens over zombie-lef niet opslaan.'
guts_creation_err: 'Kon geen zombie-lef creëren.'
guts_drop_err: 'Kon zombie-lef niet laten vallen.'
new_version_msg: '&d&lUPDATE GEVONDEN! Versie {new_version} is nu beschikbaar!'
no_update_msg: 'Geen updates beschikbaar.'
sent_torch: 'Je hebt een fakkel gestuurd naar {player}!'
sent_torch_err: 'Er is een probleem opgetreden bij het leveren van de zaklamp.'
received_torch: 'Je hebt een zaklamp gekregen van {player}'
```
{% endcode %}



</details>

