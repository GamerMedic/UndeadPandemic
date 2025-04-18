---
description: >-
  O arquivo YAML padrão para o idioma inglês. (Desenvolvido pelo Google
  Tradutor)
---

# 🇵🇹 🇵🇹 Português

<details>

<summary><code>pt.yml</code></summary>

```yaml
messages:
  # Welcome and Premium Messages
  welcome-premium: "Bem-vindo, {playerName}!"
  upgrade-premium: "Faça upgrade para o premium e obtenha benefícios exclusivos!"
  no-premium: "Esta é uma função Premium!"

  # Player Health and Effects
  thirst-warning: "Aviso: Sua sede está baixa!"
  thirst-buffer: "Sua sede está criticamente baixa! Você se sente fraco e confuso."
  water-purification: "Você purificou a água suja em água limpa!"
  analgesia-used: "Você usou Analgesia. Sua saúde foi parcialmente restaurada."
  bandage-used: "Você usou um Curativo. A regeneração de saúde foi ativada."
  antibiotics-used: "Você usou Antibióticos. Todos os efeitos negativos foram removidos!"
  adrenaline-used: "Você usou Adrenalina. Agora está com saúde total e resistência a danos por 30 segundos."
  infection-applied: "&4Você foi infectado!"

  # Zombie Guts
  zombie-guts-effect-worn-off: "O efeito das Entranhas de Zumbi desapareceu."
  zombie-guts-removed-rain: "O efeito das Entranhas de Zumbi foi removido devido à chuva."
  zombie-guts-removed-water: "O efeito das Entranhas de Zumbi foi removido ao entrar na água."
  zombie-guts-created: "*Você se cobriu com as nojentas entranhas e agora você cheira a podre!*"
  zombie-guts-chestplate: "Eu espalhei as entranhas na minha roupa... Que nojo."
  zombie-guts-status-four: "&4Isso deve durar um tempo."
  zombie-guts-status-three: "&cIsso deve durar o suficiente."
  zombie-guts-status-two: "&6Eu não tenho muito tempo com isso."
  zombie-guts-status-one: "&eIsso é apenas uma mancha, não vai durar muito."
  zombie-guts-status-zero: "&7Isso não vai adiantar, você não pode ir para lugar algum com isso."
  zombie-guts-plate-status-four: "&4Fresca e escorrendo..."
  zombie-guts-plate-status-three: "&cEscorregadia de sangue."
  zombie-guts-plate-status-two: "&6Secando. O cheiro está aumentando."
  zombie-guts-plate-status-one: "&eApodrecendo. Moscas se acumulam."
  zombie-guts-plate-status-zero: "&7Está caindo aos pedaços..."

  # Events
  bloodmoon-rises: "&4☾ A Lua de Sangue Está Subindo... ☾"
  bloodmoon-dawns: "&7☀ A Lua de Sangue desaparece com a chegada da manhã... ☀"
  bloodmoon-dread: "&7Uma sensação de medo preenche o ar..."

  # Combat and Zombies
  zombie-headshot: "&4&lTiro na cabeça!"
  zombie-bodyshot: "Você acertou o corpo do zumbi!"

  # Permissions and Restrictions
  no-permission: "Você não tem permissão para fazer isso."
  players-only-cmd: "Apenas jogadores podem executar este comando."
  player-not-found: "Jogador não encontrado."
  world-restriction-message: "Você não pode usar esta plugin no mundo atual: %world%."
  xp-restricted-world: "A coleta de XP está desabilitada neste mundo."
  xp-restricted-item: "Itens relacionados ao XP estão desabilitados neste servidor."

  # Inventory and Crafting
  torch-used: "A tocha agora está ativa e fornece visão noturna!"
  torch-out-of-power: "A tocha ficou sem energia e não pode ser usada."
  battery-empty: "Esta bateria está vazia e não pode ser usada."
  battery-transferred: "A vida da bateria foi transferida para a tocha."
  cannot-switch-during-torch-use: "Você não pode trocar de itens enquanto a tocha estiver em uso."
  crafting-success: "Você criou o item com sucesso!"
  crafting-blacklist: "&4Você não pode criar este item!"
  receipe-missing: "A receita para este item está faltando ou incompleta."
  invalid-material: "O material para este item é inválido."
  invalid-item: "Item inválido. Itens disponíveis: Adrenalina, Analgesia, Antibióticos, Curativo, Tocha, Bateria."
  invalid-qty: "Quantidade inválida. Por favor, insira um número válido."

  # Barbed Wire
  no-wire-cutters: "&cVocê precisa de cortadores de arame para remover o arame farpado!"
  hurt-by-barbed-wire: "&cVocê foi ferido pelo arame farpado!"

  # Rewards
  reward-money: "Você foi recompensado com {amount} moedas!"
  reward-items: "Você foi recompensado com x{quantity} {itemName}(s)!"

  # Configuration and Updates
  config-reload: "As configurações de configuração foram recarregadas."
  update-plots-err: "&fNão foi possível atualizar o número de parcelas de {player}."

  # Plot Management
  plots-updated: '&2O número de parcelas de {player} foi ajustado para {new-plots}. Eles agora têm {total-plots} parcelas restantes.'
  missing-plots: '&4Não foi possível recuperar o número restante de parcelas.'
  missing-plots-err: '&4Você deve escolher quantas parcelas dar a {player}.'

  # Camp Commands
  camp-cmd-no-player: '&4Você deve selecionar um jogador.'
  camp-cmd-no-amount: '&4Você deve escolher quantas parcelas dar a {player}.'
  camp-cmd-no-neg: '&eVocê não pode usar números negativos no comando /camp.'
  camp-created: '&eSeu acampamento foi criado!'
  camp-created-err: '&4Não foi possível criar o acampamento.'
  camp-destroyed: '&eSeu acampamento não está mais seguro.'
  camp-destroyed-err: '&cNão foi possível destruir seu acampamento.'
  camp-exists: '&eO acampamento não pôde ser criado porque já existe um com o mesmo nome.'
  camp-info: '------------- &c&l[Informações do Acampamento] &r&f-------------'
  camp-info-msg: 'Não foi possível recuperar o número restante de blocos.'
  camp-plot-count: 'Você tem &2{plots} &r&fparcelas restantes. Use-as com sabedoria.'
```

</details>

<details>

<summary>Legacy <code>pt.yml</code> (Pre-v3.0.0)</summary>

{% code title="pt.yml" %}
```yaml
#############################################################
#
#  Você pode obter uma tradução atualizada em https://docs.stevezr963.me/getting-started/undeadpandemic/languages/using-translations/english
#  Tradutor: MihDrix (Mundo Drix)
#  Data: 10/09/2023
#
#############################################################
head_shot_actionbar_text: '&bVocê acertou um tiro na cabeça!'
execution: '&4EXECUÇÃO!'
reload_weapon: '&c&lRECARGA DA SUA ARMA!'
weapon_jammed: '&cSua arma travou. Tente novamente.'
no_weapon: 'O item que você está segurando não é uma arma.'
no_weapon_perms: 'Você não tem permissão para usar armas.'
getting_thirty: 'Você está ficando com sede!'
thirsty: '&e&lVocê está com sede.'
died_of_thirst: '&7&oVocê morreu de sede! Tolo.'
dehydrated: '&4&lA DESIDRATAÇÃO O DEIXOU CONFUSO. BEBA ALGO, AGORA!'
no_door: '&4A porta não existe.'
broken_key: '&eOps! O cartão-chave quebrou na fechadura e agora não pode ser usado!'
infected: '&5&lVOCÊ FOI INFECTADO!!!'
no_ammo: '&g&oVocê não tem balas para recarregar.'
no_abx: '&4Você não está segurando nenhum antibiótico.'
no_adx: '&4Você não está segurando nenhuma adrenalina.'
no_bandage: '&4Você não está segurando nenhum curativo.'
no_coords: '&4Você não forneceu coordenadas completas para este cartão-chave.'
no_keycard_uses: '&4O parâmetro <uses> que você definiu é inválido. Seu cartão-chave foi criado, mas só pode ser usado uma vez.'
keycard_failed: '&4Não foi possível programar o cartão-chave para abrir portas.'
sent_ammo_cache: '&2{player} recebeu seu estoque de munições!'
sent_ammo_cache_error: '&4Não foi possível enviar um estoque de munições.'
received_ammo_cache: '&2Você recebeu um estoque de munições!'
sent_weapons_cache: '&2{player} recebeu seu estoque de armas!'
sent_weapons_cache_error: '&4Não foi possível enviar um estoque de armas.'
received_weapons_cache: '&2Você recebeu um estoque de armas!'
invalid_ammo: 'Tipo de munição inválido. Tipos válidos: <{ammoTypes}>'
weapons_disabled: '&eAs armas estão desativadas.'
weapon_not_registered: '&4{weapon} não é uma arma registrada. Esta opção é sensível a maiúsculas.'
sent_abx: '&2{player} recebeu seus antibióticos (x{amount})!'
sent_abx_err: '&4Os antibióticos não puderam ser enviados para {player}.'
sent_bandages: '&2{player} recebeu seus curativos (x{amount})!'
sent_bandages_err: '&4Os curativos não puderam ser enviados para {player}.'
sent_adx: '&2{player} recebeu sua adrenalina (x{amount})!'
sent_adx_err: '&4A adrenalina não pôde ser enviada para {player}.'
first_aid_kit_err: '&eNão foi possível criar o kit.'
invalid_first_aid_kit: '&4{kit} não é um item válido.'
safezone_exists: '&eA Zona Segura não pôde ser criada porque já existe uma com o mesmo nome.'
invalid_safezone_region: '&4Não foi possível determinar as regiões existentes.'
missing_plots: '&4Não foi possível buscar seus terrenos restantes.'
update_plots_err: '&cNão foi possível atualizar a contagem de terrenos. Por favor, avise um administrador.'
claimed_plot_err: '&cVocê não pode reivindicar terras estrangeiras.'
building_safezone: '&eConstruindo sua Zona Segura. Por favor, aguarde...'
safezone_created: '&eSua Zona Segura foi criada!'
safezone_created_err: '&4Não foi possível criar a Zona Segura.'
safezone_info: '------------- &c&l[Informações da Zona Segura] &r&f-------------'
safezone_info_msg: 'Não foi possível buscar os blocos restantes.'
safezone_plot_count: 'Você tem &2{plots} &r&fterrenos restantes. Use-os com sabedoria.'
insufficient_plots: '&fVocê não tem terrenos suficientes para expandir sua Zona Segura.'
destroy_safezone_err: '&5Esta não é a sua Zona Segura.'
safezone_destroyed: '&eSua Zona Segura não é mais segura.'
safezone_destroyed_err: '&cSua Zona Segura não pôde ser destruída.'
wrong_safezone_err: '&5Esta não é a sua Zona Segura.'
safezone_cmd_no_player: '&4Você deve selecionar um jogador.'
safezone_cmd_no_amount: '&4Você deve escolher quantos terrenos dar a {player}.'
safezone_cmd_no_neg: '&eVocê não pode usar números negativos no comando /safezone.'
cmd_no_console_err: '&4Você não pode executar este comando no console.'
cmd_give_param_err: '&4Foi fornecido um valor de quantidade inválido no comando de doação.'
cmd_help_err: '&4Uso inválido. Uso: /undeadpandemic give <{player}> <ammo|firstaid|torch|weapon> [{amount}]'
player_not_online: '&1{player} não está online.'
cmd_no_perms: '&5Você não tem permissão para usar este comando.'
invalid_args: 'Argumentos inválidos'
plot_update_err: '&fNão foi possível atualizar a contagem de terrenos de {player}.'
plots_updated: '&2A contagem de terrenos de {player} foi ajustada em {new_plots}. Agora eles têm {total_plots} terrenos restantes.'
invalid_plots: '&4{plots} não é um número válido. Você só pode usar números inteiros aqui.'
missing_plots_err: '&4Você deve escolher quantos terrenos dar a {player}.'
reload_cmd_success: 'O arquivo de configuração do UndeadPandemic foi recarregado.'
invalid_crafting_list: 'Não foi possível construir a lista de criação inválida.'
first_aid_kit_inv_err: 'Não foi possível gerar o inventário do baú do kit de primeiros socorros.'
first_aid_no_use: 'Não foi possível usar {item}.'
weapons_invalid_list: 'Lista de armas inválida.'
guts_no_change: 'Não foi possível alterar os dados de intestinos de zumbi.'
guts_save_err: 'Não foi possível salvar os dados de intestinos de zumbi.'
guts_creation_err: 'Não foi possível criar os intestinos de zumbi.'
guts_drop_err: 'Não foi possível soltar os intestinos de zumbi.'
new_version_msg: '&d&lATUALIZAÇÃO ENCONTRADA! Versão {new_version} agora está disponível!'
no_update_msg: 'Nenhuma atualização disponível.'
sent_torch: 'Você enviou uma tocha para {player}!'
sent_torch_err: 'Houve um problema na entrega da tocha.'
received_torch: 'Você recebeu uma tocha de {player}'
```
{% endcode %}



</details>
