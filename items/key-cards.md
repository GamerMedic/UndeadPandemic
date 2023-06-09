# 🔑 Key Cards

<figure><img src="../.gitbook/assets/keycard.png" alt="A 16x16 pixel white card with a short green and black stripe centred at the top of the card."><figcaption><p>Default Key Card Texture</p></figcaption></figure>

### Description

A key card is an item which can open doors. This will usually be iron doors and trapdoors as these doors require red stone functionality to open normally. However, what items can be opened is configurable.

### Obtaining Key Cards

Use the [`keycard` command](../commands/undeadpandemic/keycard.md) to craft key cards.

Key cards can only be crafted by players with the [keycard.craft permission](../permissions/permissions/undeadpandemic.keycard/undeadpandemic.keycard.craft.md).

### Using Key Cards

Players will need the [keycard.use permission](../permissions/permissions/undeadpandemic.keycard/undeadpandemic.keycard.use.md) to use key cards.

Players can use key cards by right clicking on [openable doors that are set in the config.yml](../configuration/config.yml/key-card-settings.md). Key cards will not work on any other doors.

If the door does not open when the key card is used, then the key card does not work on that door.

Players who craft key cards should define a custom [<mark style="color:red;">\[keycard description\]</mark>](../commands/undeadpandemic/keycard.md#command-structure) parameter when crafting the key card, doing so will help other players know what door will open using the key card.

### How Key Cards Work

Key cards work by opening an [openable door](../configuration/config.yml/key-card-settings.md) on the block to which the key card is programmed. The key card is not set to a specific openable door.
