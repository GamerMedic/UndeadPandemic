---
description: Zhōngwén de mòrèn YAML wénjiàn. (Yóu gǔgē fānyì tígōng zhīchí)
---

# 🇨🇳 🇨🇳 Zhōngguó rén

<details>

<summary><code>zh.yml</code></summary>

```yaml
messages:
  # Welcome and Premium Messages
  welcome-premium: "欢迎，{playerName}！"
  upgrade-premium: "升级到高级版，享受独家福利！"
  no-premium: "这是高级版功能！"

  # Player Health and Effects
  thirst-warning: "警告：你的口渴值很低！"
  thirst-buffer: "你的口渴值危机四伏！你感觉虚弱且迷茫。"
  water-purification: "你将脏水净化成了干净水！"
  analgesia-used: "你使用了止痛药。你的健康部分恢复了。"
  bandage-used: "你使用了绷带。健康恢复已启用。"
  antibiotics-used: "你使用了抗生素。所有负面效果已清除！"
  adrenaline-used: "你使用了肾上腺素。你现在恢复了满血，并且在接下来的30秒内有伤害抗性。"
  infection-applied: "&4你已被感染！"

  # Zombie Guts
  zombie-guts-effect-worn-off: "僵尸内脏效果已消失。"
  zombie-guts-removed-rain: "由于下雨，僵尸内脏效果已被移除。"
  zombie-guts-removed-water: "由于进入水中，僵尸内脏效果已被移除。"
  zombie-guts-created: "*你把恶心的僵尸内脏涂在身上，现在你闻起来像腐烂的尸体！*"
  zombie-guts-chestplate: "我把僵尸内脏涂在了衣服上... 真恶心。"
  zombie-guts-status-four: "&4这个效果应该会持续一段时间。"
  zombie-guts-status-three: "&c这个效果应该会持续足够长的时间。"
  zombie-guts-status-two: "&6我带着这个不会太久。"
  zombie-guts-status-one: "&e这只是一个污点，不能维持太久。"
  zombie-guts-status-zero: "&7这样下去也没有意义，什么地方也不能去。"
  zombie-guts-plate-status-four: "&4新鲜且滴水..."
  zombie-guts-plate-status-three: "&c血迹斑斑。"
  zombie-guts-plate-status-two: "&6正在干燥。恶臭上升。"
  zombie-guts-plate-status-one: "&e腐烂。苍蝇聚集。"
  zombie-guts-plate-status-zero: "&7正在分解..."

  # Events
  bloodmoon-rises: "&4☾ 血月升起... ☾"
  bloodmoon-dawns: "&7☀ 血月在黎明破晓时消失... ☀"
  bloodmoon-dread: "&7空气中弥漫着一股恐惧的气息..."

  # Combat and Zombies
  zombie-headshot: "&4&l爆头！"
  zombie-bodyshot: "你击中了僵尸的身体！"

  # Permissions and Restrictions
  no-permission: "你没有权限执行此操作。"
  players-only-cmd: "只有玩家可以执行此命令。"
  player-not-found: "未找到玩家。"
  world-restriction-message: "你不能在当前世界使用此插件：%world%。"
  xp-restricted-world: "在此世界中禁止收集经验值。"
  xp-restricted-item: "此服务器禁用了与经验相关的物品。"

  # Inventory and Crafting
  torch-used: "火把现在已激活，提供夜视效果！"
  torch-out-of-power: "火把电力已耗尽，无法使用。"
  battery-empty: "此电池已空，无法使用。"
  battery-transferred: "电池电量已转移到火把上。"
  cannot-switch-during-torch-use: "在使用火把时无法切换物品。"
  crafting-success: "你已成功制作该物品！"
  crafting-blacklist: "&4你不能制作这个物品！"
  receipe-missing: "此物品的配方丢失或不完整。"
  invalid-material: "该物品的材料无效。"
  invalid-item: "无效的物品。可用物品：肾上腺素、止痛药、抗生素、绷带、火把、电池。"
  invalid-qty: "数量无效。请输入一个有效的数字。"

  # Barbed Wire
  no-wire-cutters: "&c你需要 wire cutters 才能移除铁丝网！"
  hurt-by-barbed-wire: "&c你被铁丝网伤到了！"

  # Rewards
  reward-money: "你获得了 {amount} 硬币的奖励！"
  reward-items: "你获得了 x{quantity} 个 {itemName} 的奖励！"

  # Configuration and Updates
  config-reload: "配置设置已重新加载。"
  update-plots-err: "&f无法更新 {player} 的地块数量。"

  # Plot Management
  plots-updated: '&2{player} 的地块数量已调整为 {new-plots}。他们现在有 {total-plots} 个地块剩余。'
  missing-plots: '&4无法获取剩余的地块数量。'
  missing-plots-err: '&4你必须选择给 {player} 分配多少地块。'

  # Camp Commands
  camp-cmd-no-player: '&4你必须选择一个玩家。'
  camp-cmd-no-amount: '&4你必须选择给 {player} 分配多少地块。'
  camp-cmd-no-neg: '&e你不能在 /camp 命令中使用负数。'
  camp-created: '&e你的营地已创建！'
  camp-created-err: '&4无法创建营地。'
  camp-destroyed: '&e你的营地不再安全。'
  camp-destroyed-err: '&c无法销毁你的营地。'
  camp-exists: '&e无法创建营地，因为已经有一个同名的营地存在。'
  camp-info: '------------- &c&l[营地信息] &r&f-------------'
  camp-info-msg: '无法获取剩余的块数。'
  camp-plot-count: '你剩余 &2{plots} &r&f个地块。请明智使用它们。'
```

</details>

<details>

<summary>Legacy <code>zh.yml</code> (Pre-v3.0.0)</summary>

{% code title="zh.yml" %}
```yaml
head_shot_actionbar_text: "&b你完成了一次爆头！"
execution: "&4处决！"
reload_weapon: "&c&l重新装填武器！"
weapon_jammed: "&c你的枪卡壳了。请重试。"
no_weapon: "你手里拿的不是武器。"
no_weapon_perms: "你没有使用武器的权限。"
getting_thirty: "你变得口渴了！"
thirsty: "&e&l你口渴了"
died_of_thirst: "&7&你因为口渴而死亡！笨蛋。"
dehydrated: "&4&l脱水让你感到困惑。快喝点什么吧！"
no_door: "&4门不存在。"
broken_key: "&e糟糕！钥匙卡断裂在锁里，现在无法使用！"
infected: "&5&l你已经被感染了！！！"
no_ammo: "&g&o你没有任何子弹来装填。"
no_abx: "&4你没有携带任何抗生素。"
no_adx: "&4你没有携带任何肾上腺素。"
no_bandage: "&4你没有携带任何绷带。"
no_coords: "&4你没有提供完整的坐标信息以使用这张钥匙卡。"
no_keycard_uses: "&4你设置的<uses>参数无效。你的钥匙卡已创建，但只能使用一次。"
keycard_failed: "&4无法编程钥匙卡以打开门。"
sent_ammo_cache: "&2{player}已收到他们的弹药储藏！"
sent_ammo_cache_error: "&4无法发送弹药储藏。"
received_ammo_cache: "&2你已收到一个弹药储藏！"
sent_weapons_cache: "&2{player} 已收到他们的武器储藏！"
sent_weapons_cache_error: "&4无法发送武器储藏。"
received_weapons_cache: "&2你已收到一个武器储藏！"
invalid_ammo: "无效的弹药类型。有效类型: <{ammoTypes}>"
weapons_disabled: "&e武器已禁用。"
weapon_not_registered: "&4{weapon} 不是已注册的武器。此选项区分大小写。"
sent_abx: "&2{player} 已收到他们的抗生素（x{amount}）！"
sent_abx_err: "&4无法将抗生素发送给 {player}。"
sent_bandages: "&2{player} 已收到绷带（x{amount}）！"
sent_bandages_err: "&4无法将绷带发送给 {player}。"
sent_adx: "&2{player} 已收到肾上腺素（x{amount}）！"
sent_adx_err: "&4无法将肾上腺素发送给 {player}。"
first_aid_kit_err: "&e无法创建急救包。"
invalid_first_aid_kit: "&4{kit} 不是有效的物品。"
safezone_exists: "&e无法创建安全区域，因为已存在同名区域。"
invalid_safezone_region: "&4无法确定现有区域。"
missing_plots: "&4无法获取您剩余的地块数。"
update_plots_err: "&c无法更新地块计数，请通知管理员。"
claimed_plot_err: "&c您不能申领他人土地。"
building_safezone: "&e正在建立您的安全区域，请稍候..."
safezone_created: "&e您的安全区域已创建！"
safezone_created_err: "&4无法创建安全区域。"
safezone_info: "------------- &c&l[安全区域信息] &r&f-------------"
safezone_info_msg: "无法获取您剩余的方块数。"
safezone_plot_count: "你还有 &2{plots} &r&f个土地可用。请明智使用。"
insufficient_plots: "你没有足够的土地来扩展你的安全区域。"
destroy_safezone_err: "&5这不是你的安全区域。"
safezone_destroyed: "&e你的安全区域不再安全。"
safezone_destroyed_err: "&c无法销毁你的安全区域。"
wrong_safezone_err: "&5这不是你的安全区域。"
safezone_cmd_no_player: "&4你必须选择一个玩家。"
safezone_cmd_no_amount: "&4你必须选择给予 {player} 多少个土地块数量。"
safezone_cmd_no_neg: "&e在 /safezone 命令中不能使用负数。"
cmd_no_console_err: "&4你不能从控制台执行此命令。"
cmd_give_param_err: "&4给予命令中提供了一个无效的数量值。"
cmd_help_err: "&4无效用法。用法: /undeadpandemic give <{player}> <firstaid|torch> [{amount}]"
player_not_online: "&1{player} 不在线。"
cmd_no_perms: "&5你没有使用这个命令的权限。"
invalid_args: "无效参数"
plot_update_err: "&f无法更新 {player} 的土地块计数。"
plots_updated: "&2{player} 的土地块数已调整为 {new_plots}。他们现在剩余 {total_plots} 个土地块。"
invalid_plots: "&4{plots} 不是一个有效的数字。在这里，你只能使用整数。"
missing_plots_err: "&4你必须选择给予 {player} 多少个土地块数量。"
reload_cmd_success: "UndeadPandemic 配置文件已重新加载。"
invalid_crafting_list: "无法构建无效的合成列表。"
first_aid_kit_inv_err: "无法生成急救包箱子的物品栏。"
first_aid_no_use: "无法使用 {item}。"
weapons_invalid_list: "无效的武器列表。"
guts_no_change: "无法更改僵尸内脏数据。"
guts_save_err: "无法保存僵尸内脏数据。"
guts_creation_err: "无法创建僵尸内脏。"
guts_drop_err: "无法丢弃僵尸内脏。"
new_version_msg: "&d&l发现更新！版本 {new_version} 已可用！"
no_update_msg: "无可用更新。"
sent_torch: "你已发送一个火把给 {player}！"
sent_torch_err: "发送火把时出现问题。"
received_torch: "你接收到了一个火把，来自于 {player}"
```
{% endcode %}



</details>
