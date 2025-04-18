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
  # Welcome and Premium Messages
  welcome-premium: "Willkommen, {playerName}!"
  upgrade-premium: "Upgrade auf Premium für exklusive Vorteile!"
  no-premium: "Dies ist eine Premium-Funktion!"

  # Player Health and Effects
  thirst-warning: "Warnung: Dein Durst ist niedrig!"
  thirst-buffer: "Dein Durst ist kritisch niedrig! Du fühlst dich schwach und verwirrt."
  water-purification: "Du hast das schmutzige Wasser in sauberes Wasser umgewandelt!"
  analgesia-used: "Du hast Analgesie verwendet. Deine Gesundheit wurde teilweise wiederhergestellt."
  bandage-used: "Du hast ein Verband verwendet. Die Gesundheitsregeneration wurde aktiviert."
  antibiotics-used: "Du hast Antibiotika verwendet. Alle negativen Effekte wurden entfernt."
  adrenaline-used: "Du hast Adrenalin verwendet. Du bist nun bei voller Gesundheit und hast für 30 Sekunden Schadensresistenz."
  infection-applied: "&4Du wurdest infiziert!"

  # Zombie Guts
  zombie-guts-effect-worn-off: "Der Zombie-Gutseffekt ist abgeklungen."
  zombie-guts-removed-rain: "Der Zombie-Gutseffekt wurde durch den Regen entfernt."
  zombie-guts-removed-water: "Der Zombie-Gutseffekt wurde durch das Eintauchen ins Wasser entfernt."
  zombie-guts-created: "*Du hast dich mit den ekelhaften Eingeweiden bedeckt und riechst jetzt faul!*"
  zombie-guts-chestplate: "Ich habe mein Oberteil mit Eingeweiden beschmiert... Eklig."
  zombie-guts-status-four: "&4Das sollte eine Weile halten."
  zombie-guts-status-three: "&cDas sollte lange genug halten."
  zombie-guts-status-two: "&6Ich werde nicht lange mit diesem Geruch leben."
  zombie-guts-status-one: "&eDas ist nur ein Klecks, es wird nicht lange halten."
  zombie-guts-status-zero: "&7Es hat keinen Sinn, mit diesem Geruch noch irgendwo hinzugehen."
  zombie-guts-plate-status-four: "&4Frisch und tropfend..."
  zombie-guts-plate-status-three: "&cRutschig vom Blut."
  zombie-guts-plate-status-two: "&6Trocknend. Der Gestank steigt."
  zombie-guts-plate-status-one: "&eZerfallend. Fliegen sammeln sich."
  zombie-guts-plate-status-zero: "&7Fällt auseinander..."

  # Events
  bloodmoon-rises: "&4☾ Der Blutmond steigt... ☾"
  bloodmoon-dawns: "&7☀ Der Blutmond vergeht, als die Morgendämmerung anbricht... ☀"
  bloodmoon-dread: "&7Ein Gefühl der Angst liegt in der Luft..."

  # Combat and Zombies
  zombie-headshot: "&4&lKopfschuss!"
  zombie-bodyshot: "Du hast den Zombie am Körper getroffen!"

  # Permissions and Restrictions
  no-permission: "Du hast keine Berechtigung, dies zu tun."
  players-only-cmd: "Nur Spieler können diesen Befehl ausführen."
  player-not-found: "Spieler konnte nicht gefunden werden."
  world-restriction-message: "Du kannst dieses Plugin in der aktuellen Welt nicht verwenden: %world%."
  xp-restricted-world: "XP-Sammlung ist in dieser Welt deaktiviert."
  xp-restricted-item: "XP-bezogene Gegenstände sind auf diesem Server deaktiviert."

  # Inventory and Crafting
  torch-used: "Die Fackel ist jetzt aktiv und bietet Nachtsicht!"
  torch-out-of-power: "Die Fackel hat keine Batterie mehr und kann nicht mehr verwendet werden."
  battery-empty: "Dieser Akku ist leer und kann nicht verwendet werden."
  battery-transferred: "Batterieleistung wurde auf die Fackel übertragen."
  cannot-switch-during-torch-use: "Du kannst während der Verwendung der Fackel keine Gegenstände wechseln."
  crafting-success: "Du hast den Gegenstand erfolgreich hergestellt!"
  crafting-blacklist: "&4Du kannst diesen Gegenstand nicht herstellen!"
  receipe-missing: "Das Rezept für diesen Gegenstand fehlt oder ist unvollständig."
  invalid-material: "Das Material für diesen Gegenstand ist ungültig."
  invalid-item: "Ungültiger Gegenstand. Verfügbare Gegenstände: Adrenalin, Analgesie, Antibiotika, Verband, Fackel, Batterie."
  invalid-qty: "Ungültige Menge. Bitte gib eine gültige Zahl ein."

  # Barbed Wire
  no-wire-cutters: "&cDu benötigst Drahtschneider, um Stacheldraht zu entfernen!"
  hurt-by-barbed-wire: "&cDu wurdest vom Stacheldraht verletzt!"

  # Rewards
  reward-money: "Du wurdest mit {amount} Münzen belohnt!"
  reward-items: "Du wurdest mit x{quantity} {itemName}(s) belohnt!"

  # Configuration and Updates
  config-reload: "Die Konfigurationseinstellungen wurden neu geladen."
  update-plots-err: "&fEs konnte {player}'s Plot-Anzahl nicht aktualisiert werden."

  # Plot Management
  plots-updated: '&2{player} Plot-Anzahl wurde um {new-plots} angepasst. Sie haben jetzt {total-plots} Plots übrig.'
  missing-plots: '&4Konnte deine verbleibenden Plots nicht abrufen.'
  missing-plots-err: '&4Du musst auswählen, wie viele Plots du {player} geben möchtest.'

  # Camp Commands
  camp-cmd-no-player: '&4Du musst einen Spieler auswählen.'
  camp-cmd-no-amount: '&4Du musst auswählen, wie viele Plots du {player} geben möchtest.'
  camp-cmd-no-neg: '&eDu kannst keine negativen Zahlen im /camp Befehl verwenden.'
  camp-created: '&eDein Lager wurde erstellt!'
  camp-created-err: '&4Das Lager konnte nicht erstellt werden.'
  camp-destroyed: '&eDein Lager ist nicht mehr sicher.'
  camp-destroyed-err: '&cDein Lager konnte nicht zerstört werden.'
  camp-exists: '&eDas Lager konnte nicht erstellt werden, weil ein Lager mit demselben Namen bereits existiert.'
  camp-info: '------------- &c&l[Lager Info] &r&f-------------'
  camp-info-msg: 'Konnte deine verbleibenden Blöcke nicht abrufen.'
  camp-plot-count: 'Du hast &2{plots} &r&fPlots übrig. Verwende sie weise.'
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
