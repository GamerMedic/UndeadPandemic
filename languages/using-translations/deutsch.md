---
description: >-
  Die YAML-Standarddatei für die deutsche Sprache. (Von Google Translate
  bereitgestellt)
---

# 🇩🇪 🇩🇪 Deutsch

<details>

<summary>de.yml</summary>

```yaml
messages:
  zombie-guts-effect-worn-off: "Der Zombie-Eingeweide-Effekt ist abgelaufen."
  zombie-guts-removed-rain: "Der Zombie-Eingeweide-Effekt wurde aufgrund des Regens entfernt."
  zombie-guts-removed-water: "Der Zombie-Eingeweide-Effekt wurde durch das Betreten von Wasser entfernt."
  welcome-premium: "Willkommen, {playerName}!"
  upgrade-premium: "Upgrade auf Premium für exklusive Vorteile!"
  no-premium: "Dies ist eine Premium-Funktion!"
  thirst-warning: "Warnung: Dein Durst ist niedrig!"
  thirst-buffer: "Dein Durst ist kritisch niedrig! Du fühlst dich schwach und verwirrt."
  water-purification: "Du hast das schmutzige Wasser in sauberes Wasser gereinigt!"
  zombie-headshot: "Du hast den Kopf des Zombies getroffen!"
  zombie-bodyshot: "Du hast den Körper des Zombies getroffen!"
  infection-applied: "&4Du wurdest infiziert!"
  world-restriction-message: "Du kannst dieses Plugin nicht in der aktuellen Welt verwenden: %world%."
  xp-restricted-world: "Das Sammeln von Erfahrungspunkten ist in dieser Welt deaktiviert."
  xp-restricted-item: "XP-bezogene Gegenstände sind auf diesem Server deaktiviert."
  torch-used: "Die Fackel ist jetzt aktiv und bietet Nachtsicht!"
  torch-out-of-power: "Die Fackel hat keine Energie mehr und kann nicht verwendet werden."
  battery-empty: "Diese Batterie ist leer und kann nicht verwendet werden."
  battery-transferred: "Die Batterieleistung wurde auf die Fackel übertragen."
  cannot-switch-during-torch-use: "Du kannst keine Gegenstände wechseln, während die Fackel verwendet wird."
  analgesia-used: "Du hast Analgesia verwendet. Deine Gesundheit wurde teilweise wiederhergestellt."
  bandage-used: "Du hast einen Verband benutzt. Gesundheitsregeneration wurde aktiviert."
  antibiotics-used: "Du hast Antibiotika verwendet. Alle negativen Effekte wurden entfernt."
  adrenaline-used: "Du hast Adrenalin verwendet. Du bist jetzt vollständig geheilt und hast 30 Sekunden lang Schadensresistenz."
  crafting-success: "Du hast das Item erfolgreich hergestellt!"
  receipe-missing: "Das Rezept für dieses Item fehlt oder ist unvollständig."
  invalid-material: "Das Material für dieses Item ist ungültig."
  config-reload: "Die Konfigurationseinstellungen wurden neu geladen."
  no-permission: "Du hast keine Berechtigung, diesen Befehl auszuführen."
  players-only-cmd: "Nur Spieler können diesen Befehl ausführen."
  player-not-found: "Spieler konnte nicht gefunden werden."
  invalid-item: "Ungültiges Item. Verfügbare Items: Adrenalin, Analgesia, Antibiotika, Verband, Fackel, Batterie."
  invalid-qty: "Ungültige Menge. Bitte gib eine gültige Zahl ein."
  no-wire-cutters: "&cDu benötigst Drahtschneider, um Stacheldraht zu entfernen!"
  hurt-by-barbed-wire: "&cDu wurdest durch den Stacheldraht verletzt!"
  reward-money: "Du hast {amount} Münzen erhalten!"
  reward-items: "Du hast x{quantity} {itemName}(s) erhalten!"

```

</details>

<details>

<summary>Legacy <code>de.yml</code> (Pre-v3.0.0)</summary>

{% code title="de.yml" overflow="wrap" lineNumbers="true" %}
```yaml
#############################################################
#
#  Sie können eine aktualisierte Übersetzung von erhalten https://docs.stevezr963.me/getting-started/undeadpandemic/languages/using-translations/deutsch
#
#############################################################
head_shot_actionbar_text: '&bDu hast einen Kopfschuss!'
execution: '&4HINRICHTUNG!'
reload_weapon: '&c&lLADEN SIE IHRE WAFFE NEU!'
weapon_jammed: '&cIhre Waffe klemmt. Versuchen Sie es nochmal.'
no_weapon: 'Der Gegenstand, den Sie halten, ist keine Waffe.'
no_weapon_perms: 'Sie haben keine Erlaubnis, Waffen zu benutzen.'
getting_thirty: 'Du wirst durstig!'
thirsty: '&e&lDu hast Durst!'
died_of_thirst: '&7&oDu bist verdurstet! Dummkopf.'
dehydrated: '&4&lSIE SIND VERWIRKLICH, WEIL SIE DEHYDRATIERT SIND. TRINKEN SIE JETZT ETWAS!'
no_door: '&4Tür existiert nicht.'
broken_key: '&eHoppla! Die Schlüsselkarte ist im Schloss eingeschnappt und ist nun unbrauchbar!'
infected: '&5&lDU WURDE VON EINEM ZOMBIE INFIZIERT!!!'
no_ammo: '&g&oSie haben keine Kugeln zum Nachladen.'
no_abx: '&4Sie haben keine Antibiotika in der Hand.'
no_adx: '&4Sie halten kein Adrenalin in der Hand.'
no_bandage: '&4You are not holding any bandages.'
no_coords: '&4Sie haben keine vollständigen Koordinaten für diese Schlüsselkarte angegeben.'
no_keycard_uses: '&4Der von Ihnen festgelegte <uses>-Parameter war ungültig. Ihre Schlüsselkarte wurde erstellt, kann aber nur einmal verwendet werden.'
keycard_failed: '&4Die Schlüsselkarte konnte nicht zum Öffnen von Türen programmiert werden.'
sent_ammo_cache: '&2{player} hat den Munitions-Cache erhalten!'
sent_ammo_cache_error: '&4Ein Munitions-Cache konnte nicht gesendet werden.'
received_ammo_cache: '&2Du hast einen Munitions-Cache erhalten!'
sent_weapons_cache: '&2{player} hat den Waffen-Cache erhalten!'
sent_weapons_cache_error: '&4Der Waffen-Cache konnte nicht gesendet werden.'
received_weapons_cache: '&2Du hast einen Waffen-Cache erhalten!'
invalid_ammo: 'Ungültiger Munitionstyp. Gültige Typen: <{ammoTypes}>'
weapons_disabled: '&eWaffen sind deaktiviert.'
weapon_not_registered: '&4{weapon} ist keine registrierte Waffe. Bei dieser Option wird zwischen Groß- und Kleinschreibung unterschieden.'
sent_abx: '&2{player} hat das Antibiotikum bekommen (x{amount})!'
sent_abx_err: '&4Antibiotika konnten nicht versendet werden {player}.'
sent_bandages: '&2{player} hat die Verband(e) erhalten (x{amount})!'
sent_bandages_err: '&4Verband(e) konnten nicht an gesendet werden {player}.'
sent_adx: '&2{player} hat das Adrenalin erhalten (x{amount})!'
sent_adx_err: '&4Adrenalin konnte nicht an geschickt werden {player}.'
first_aid_kit_err: '&eBausatz konnte nicht erstellt werden.'
invalid_first_aid_kit: '&4{kit} ist kein gültiges Objekt.'
safezone_exists: '&eSichere Zone konnte nicht erstellt werden, da bereits eine Zone mit demselben Namen vorhanden ist.'
invalid_safezone_region: '&4Vorhandene Regionen konnten nicht ermittelt werden.'
missing_plots: '&4Ihre verbleibenden Plots konnten nicht abgerufen werden.'
update_plots_err: '&cPlotanzahl konnte nicht aktualisiert werden. Bitte benachrichtige einen Admin.'
claimed_plot_err: '&cSie können kein fremdes Land beanspruchen.'
building_safezone: '&eAufbau Ihrer sicheren Zone. Warten Sie mal...'
safezone_created: '&eIhre sichere Zone wurde erstellt!'
safezone_created_err: '&4Sichere Zone konnte nicht erstellt werden.'
safezone_info: '------------- &c&l[Informationen zu SafeZones] &r&f-------------'
safezone_info_msg: 'Ihre verbleibenden Blöcke konnten nicht abgerufen werden.'
safezone_plot_count: 'Sie haben noch &2{plots} &r&fplots übrig. Nutze sie weise.'
insufficient_plots: '&fSie haben nicht genügend Fläche, um Ihre sichere Zone zu erweitern.'
destroy_safezone_err: '&5Dies ist nicht Ihre sichere Zone.'
safezone_destroyed: '&eIhre sichere Zone ist nicht mehr sicher.'
safezone_destroyed_err: '&cIhre Sicherheitszone konnte nicht zerstört werden.'
wrong_safezone_err: '&5Dies ist nicht Ihre sichere Zone.'
safezone_cmd_no_player: '&4Sie müssen einen Spieler auswählen.'
safezone_cmd_no_amount: '&4Sie müssen wählen, wie vielen Zonen Sie geben möchten {player}.'
safezone_cmd_no_neg: '&eSie können im Befehl /safezone keine negativen Zahlen verwenden.'
cmd_no_console_err: '&4Sie können diesen Befehl nicht über die Konsole ausführen.'
cmd_give_param_err: '&4Im Give-Befehl wurde ein ungültiger Mengenwert angegeben.'
cmd_help_err: '&4Ungültige Verwendung. Verwendung: /undeadpandemic give <{player}> <ammo|firstaid|torch|weapon> [{amount}]'
player_not_online: '&1{player} ist nicht online.'
cmd_no_perms: '&5Sie sind nicht berechtigt, diesen Befehl zu verwenden.'
invalid_args: 'Ungültige Argumente'
plot_update_err: '&fDie Plotanzahl von {player} konnte nicht aktualisiert werden.'
plots_updated: '&2Die Plotanzahl von {player} wurde von {new_plots} angepasst. Der Spieler hat jetzt noch {total_plots} Parzellen übrig.'
invalid_plots: '&4{plots} ist keine gültige Zahl. Sie können hier nur ganze Zahlen verwenden.'
missing_plots_err: '&4Sie müssen auswählen, wie viele Zonen Sie {player} geben möchten.'
reload_cmd_success: 'Die UndeadPandemic-Konfigurationsdatei wurde neu geladen.'
invalid_crafting_list: 'Ungültige Handwerksliste konnte nicht erstellt werden.'
first_aid_kit_inv_err: 'Erste-Hilfe-Kasteninventar konnte nicht generiert werden.'
first_aid_no_use: '{item} konnte nicht verwendet werden.'
weapons_invalid_list: 'Waffenliste ungültig.'
guts_no_change: 'Zombie-Eingeweide-Daten konnten nicht geändert werden.'
guts_save_err: 'Zombie-Eingeweide-Daten konnten nicht gespeichert werden.'
guts_creation_err: 'Konnte Zombie-Eingeweide nicht erschaffen.'
guts_drop_err: 'Konnte keine Zombie-Eingeweide fallen lassen.'
new_version_msg: '&d&lUPDATE GEFUNDEN! Version {new_version} ist jetzt verfügbar!'
no_update_msg: 'Keine Updates verfügbar.'
sent_torch: 'Du hast eine Taschenlampe geschickt {player}!'
sent_torch_err: 'Bei der Lieferung der Taschenlampe ist ein Problem aufgetreten.'
received_torch: 'Du hast eine Taschenlampe von erhalten {player}'
```
{% endcode %}



</details>
