---
description: >-
  El archivo YAML predeterminado para el idioma inglés. (Traducido usando el
  Traductor de Google)
---

# 🇪🇸 🇪🇸 Español

<details>

<summary><code>es.yml</code></summary>

```yaml
messages:
  # Welcome and Premium Messages
  welcome-premium: "¡Bienvenido, {playerName}!"
  upgrade-premium: "¡Mejora a premium para obtener beneficios exclusivos!"
  no-premium: "¡Esta es una función Premium!"

  # Player Health and Effects
  thirst-warning: "¡Advertencia: Tu sed está baja!"
  thirst-buffer: "¡Tu sed está críticamente baja! Te sientes débil y confundido."
  water-purification: "¡Has purificado el agua sucia en agua limpia!"
  analgesia-used: "Has usado Analgesia. Tu salud ha sido parcialmente restaurada."
  bandage-used: "Has usado un Vendaje. La regeneración de salud ha sido activada."
  antibiotics-used: "Has usado Antibióticos. ¡Se han eliminado todos los efectos negativos!"
  adrenaline-used: "Has usado Adrenalina. Ahora estás a plena salud y con resistencia al daño durante 30 segundos."
  infection-applied: "&4¡Has sido infectado!"

  # Zombie Guts
  zombie-guts-effect-worn-off: "El efecto de las Tripas de Zombie ha desaparecido."
  zombie-guts-removed-rain: "El efecto de las Tripas de Zombie ha sido removido por la lluvia."
  zombie-guts-removed-water: "El efecto de las Tripas de Zombie ha sido removido por entrar al agua."
  zombie-guts-created: "*¡Te has cubierto con las asquerosas tripas y ahora hueles a podredumbre!*"
  zombie-guts-chestplate: "Me he untado la camiseta con tripas... Qué asco."
  zombie-guts-status-four: "&4Esto debería durar un rato."
  zombie-guts-status-three: "&cEsto debería durar lo suficiente."
  zombie-guts-status-two: "&6No me queda mucho tiempo con esto."
  zombie-guts-status-one: "&eEsto es solo un poco, no durará mucho."
  zombie-guts-status-zero: "&7No tiene sentido ir a ningún lado con esto."
  zombie-guts-plate-status-four: "&4Fresco y goteando..."
  zombie-guts-plate-status-three: "&cResbaloso con sangre."
  zombie-guts-plate-status-two: "&6Secándose. El olor aumenta."
  zombie-guts-plate-status-one: "&eDescomponiéndose. Las moscas se agrupan."
  zombie-guts-plate-status-zero: "&7Deshaciéndose..."

  # Events
  bloodmoon-rises: "&4☾ La Luna Sangrienta se eleva... ☾"
  bloodmoon-dawns: "&7☀ La Luna Sangrienta desaparece cuando amanece... ☀"
  bloodmoon-dread: "&7Un sentimiento de pavor llena el aire..."

  # Combat and Zombies
  zombie-headshot: "&4&l¡Disparo a la cabeza!"
  zombie-bodyshot: "¡Has golpeado el cuerpo del zombie!"

  # Permissions and Restrictions
  no-permission: "No tienes permiso para hacer eso."
  players-only-cmd: "Solo los jugadores pueden ejecutar este comando."
  player-not-found: "No se pudo encontrar al jugador."
  world-restriction-message: "No puedes usar este plugin en el mundo actual: %world%."
  xp-restricted-world: "La recolección de XP está deshabilitada en este mundo."
  xp-restricted-item: "Los objetos relacionados con XP están deshabilitados en este servidor."

  # Inventory and Crafting
  torch-used: "¡La antorcha está activa y proporciona visión nocturna!"
  torch-out-of-power: "La antorcha se ha quedado sin batería y no se puede usar."
  battery-empty: "Esta batería está vacía y no se puede usar."
  battery-transferred: "La batería se ha transferido a la antorcha."
  cannot-switch-during-torch-use: "No puedes cambiar de objeto mientras la antorcha está en uso."
  crafting-success: "¡Has creado el objeto con éxito!"
  crafting-blacklist: "&4¡No puedes crear este objeto!"
  receipe-missing: "La receta para este objeto falta o está incompleta."
  invalid-material: "El material para este objeto no es válido."
  invalid-item: "Objeto inválido. Objetos disponibles: Adrenalina, Analgesia, Antibióticos, Vendaje, Antorcha, Batería."
  invalid-qty: "Cantidad inválida. Por favor ingresa un número válido."

  # Barbed Wire
  no-wire-cutters: "&c¡Necesitas cortadores de alambre para quitar el alambre de púas!"
  hurt-by-barbed-wire: "&c¡Te has lastimado con el alambre de púas!"

  # Rewards
  reward-money: "¡Has sido recompensado con {amount} monedas!"
  reward-items: "¡Has sido recompensado con x{quantity} {itemName}(s)! "

  # Configuration and Updates
  config-reload: "La configuración ha sido recargada."
  update-plots-err: "&fNo se pudo actualizar el número de parcelas de {player}."

  # Plot Management
  plots-updated: '&2La cuenta de parcelas de {player} ha sido ajustada por {new-plots}. Ahora tiene {total-plots} parcelas restantes.'
  missing-plots: '&4No se pudo obtener el número restante de parcelas.'
  missing-plots-err: '&4Debes elegir cuántas parcelas dar a {player}.'

  # Camp Commands
  camp-cmd-no-player: '&4Debes seleccionar un jugador.'
  camp-cmd-no-amount: '&4Debes elegir cuántas parcelas darle a {player}.'
  camp-cmd-no-neg: '&eNo puedes usar números negativos en el comando /camp.'
  camp-created: '&e¡Tu campamento ha sido creado!'
  camp-created-err: '&4No se pudo crear el campamento.'
  camp-destroyed: '&eTu campamento ya no es seguro.'
  camp-destroyed-err: '&cNo se pudo destruir tu campamento.'
  camp-exists: '&eNo se pudo crear el campamento porque ya existe uno con el mismo nombre.'
  camp-info: '------------- &c&l[Información del Campamento] &r&f-------------'
  camp-info-msg: 'No se pudo obtener la cantidad restante de bloques.'
  camp-plot-count: 'Te quedan &2{plots} &r&fparcelas. Úsalas sabiamente.'
```

</details>

<details>

<summary>Legacy <code>es.yml</code> (Pre-v3.0.0)</summary>

{% code title="es.yml" %}
```yaml
#############################################################
#
#  Puede obtener una traducción actualizada en https://docs.stevezr963.me/getting-started/undeadpandemic/languages/using-translations/espanol
#
#############################################################
head_shot_actionbar_text: '&b¡Obtuviste un disparo en la cabeza!'
execution: '&4¡EJECUCIÓN!'
reload_weapon: '&c&lRECARGA TU ARMA!'
weapon_jammed: '&cTu arma se atascó. Inténtalo de nuevo.'
no_weapon: 'El objeto que estás sosteniendo no es un arma.'
no_weapon_perms: 'No tienes permiso para usar armas.'
getting_thirty: '¡Te estás quedando sediento!'
thirsty: '&e&lTienes sed'
died_of_thirst: '&7&o¡Has muerto de sed! Tonto.'
dehydrated: '&4&lLA DESHIDRATACIÓN TE HA HECHO CONFUNDIR. BEBE ALGO, ¡AHORA!'
no_door: '&4La puerta no existe.'
broken_key: '&e¡Ups! ¡La tarjeta clave se rompió en la cerradura y ahora no se puede usar!'
infected: '&5&l¡HAS SIDO INFECTADO!'
no_ammo: '&g&oNo tienes balas para recargar.'
no_abx: '&4No tienes ningún antibiótico en tus manos.'
no_adx: '&4No tienes ninguna adrenalina en tus manos.'
no_bandage: '&4No tienes ninguna venda en tus manos.'
no_coords: '&4No has proporcionado las coordenadas completas para esta tarjeta clave.'
no_keycard_uses: '&4El parámetro <uses> que estableciste no es válido. Se ha creado tu tarjeta clave, pero solo se puede usar una vez.'
keycard_failed: '&4No se pudo programar la tarjeta clave para abrir las puertas.'
sent_ammo_cache: '&2¡{player} ha recibido su cache de municiones!'
sent_ammo_cache_error: '&4No se pudo enviar un cache de municiones.'
received_ammo_cache: '&2¡Has recibido un cache de municiones!'
sent_weapons_cache: '&2¡{player} ha recibido su cache de armas!'
sent_weapons_cache_error: '&4No se pudo enviar un cache de armas.'
received_weapons_cache: '&2¡Has recibido un cache de armas!'
invalid_ammo: 'Tipo de munición no válido. Tipos válidos: <{ammoTypes}>'
weapons_disabled: '&eLas armas están desactivadas.'
weapon_not_registered: '&4{weapon} no es un arma registrada. Esta opción distingue entre mayúsculas y minúsculas.'
sent_abx: '&2¡{player} ha recibido sus antibióticos (x{amount})!'
sent_abx_err: '&4No se pudieron enviar los antibióticos a {player}.'
sent_bandages: '&2¡{player} ha recibido su(s) venda(s) (x{amount})!'
sent_bandages_err: '&4No se pudieron enviar las vendas a {player}.'
sent_adx: '&2¡{player} ha recibido su adrenalina (x{amount})!'
sent_adx_err: '&4No se pudo enviar la adrenalina a {player}.'
first_aid_kit_err: '&eNo se pudo crear el kit.'
invalid_first_aid_kit: '&4{kit} no es un objeto válido.'
safezone_exists: '&eNo se pudo crear la Zona Segura porque ya existe una con el mismo nombre.'
invalid_safezone_region: '&4No se pudieron determinar las regiones existentes.'
missing_plots: '&4No se pudieron obtener las parcelas restantes.'
update_plots_err: '&cNo se pudieron actualizar las parcelas. Por favor, avisa a un administrador.'
claimed_plot_err: '&cNo puedes reclamar tierra ajena.'
building_safezone: '&eConstruyendo tu Zona Segura. Por favor, espera...'
safezone_created: '&e¡Se ha creado tu Zona Segura!'
safezone_created_err: '&4No se pudo crear la Zona Segura.'
safezone_info: '------------- &c&l[Información de Zonas Seguras] &r&f-------------'
safezone_info_msg: 'No se pudieron obtener tus bloques restantes.'
safezone_plot_count: 'Te quedan &2{plots} &r&fparcelas. Úsalas sabiamente.'
insufficient_plots: '&fNo tienes suficientes parcelas para ampliar tu Zona Segura.'
destroy_safezone_err: '&5Esta no es tu Zona Segura.'
safezone_destroyed: '&eTu Zona Segura ya no es segura.'
safezone_destroyed_err: '&cNo se pudo destruir tu Zona Segura.'
wrong_safezone_err: '&5Esta no es tu Zona Segura.'
safezone_cmd_no_player: '&4Debes seleccionar un jugador.'
safezone_cmd_no_amount: '&4Debes elegir cuántas parcelas darle a {player}.'
safezone_cmd_no_neg: '&eNo puedes usar números negativos en el comando /zona-segura.'
cmd_no_console_err: '&4No puedes ejecutar este comando desde la consola.'
cmd_give_param_err: '&4Se proporcionó un valor de cantidad no válido en el comando dar.'
cmd_help_err: '&4Uso incorrecto. Uso: /undeadpandemic give <{player}> <ammo|firstaid|torch|weapon> [{amount}]'
player_not_online: '&1{player} no está en línea.'
cmd_no_perms: '&5No tienes permiso para usar este comando.'
invalid_args: 'Argumentos no válidos'
plot_update_err: '&fNo se pudo actualizar el recuento de parcelas de {player}.'
plots_updated: '&2Se ha ajustado el recuento de parcelas de {player} en {new_plots}. Ahora tienen {total_plots} parcelas restantes.'
invalid_plots: '&4{plots} no es un número válido. Solo puedes usar números enteros aquí.'
missing_plots_err: '&4Debes elegir cuántas parcelas darle a {player}.'
reload_cmd_success: 'Se ha recargado el archivo de configuración de UndeadPandemic.'
invalid_crafting_list: 'No se pudo crear una lista de fabricación no válida.'
first_aid_kit_inv_err: 'No se pudo generar el inventario del cofre del botiquín.'
first_aid_no_use: 'No se pudo usar {item}.'
weapons_invalid_list: 'Lista de armas no válida.'
guts_no_change: 'No se pudo cambiar los datos de guts.'
guts_save_err: 'No se pudo guardar los datos de guts.'
guts_creation_err: 'No se pudo invocar al zombie guts.'
guts_drop_err: 'No se obtuvo drop del zombie guts.'
new_version_msg: '&d&l¡ACTUALIZACIÓN ENCONTRADA! ¡Versión {new_version} ya está disponible!'
no_update_msg: 'No hay actualizaciones disponibles.'
sent_torch: '¡Has enviado una linterna a {player}!'
sent_torch_err: 'Hubo un problema al entregar la linterna.'
received_torch: 'Has recibido una linterna de {player}'
```
{% endcode %}



</details>
