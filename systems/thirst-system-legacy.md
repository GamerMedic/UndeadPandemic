---
description: What is the thirst system? And how does it work?
---

# Thirst System (Legacy)

{% hint style="danger" %}
The thirst system changed drastically in v2.6.0. Please visit the [Health System](health-system/) for more information.
{% endhint %}

### What is the thirst system?

The thirst system allows players to experience thirst within the game.

### How does the thirst system work?

#### Dehydration

When enabled, the XP level bar will be set to 80% by default, and will decrease every x seconds. The rate of dehydration is set by the `dehydration_rate` setting.

#### Becoming Unwell

The player will be alerted when they start to become dehydrated. They will get a message when they hit 50% and 25%.

When a player hits 5% thirst, dehydration will start taking effect. The player will become confused and lethargic, altering their state of mind.

#### Rehydration

A player can restore their hydration levels, and become well again, by using consumables. Consumables will replenish their hydration level according to the [Consumables setting](../configuration/config.yml/thirst-settings.md).

### Consequences

The main, and most significant, consequence of using the thirst system is that players can easily obtain XP by using consumables.

It is, therefore, recommended that you <mark style="color:red;">**disable the**</mark> [_<mark style="color:red;">**enchant settings**</mark>_](../configuration/config.yml/enchant-settings.md) while using the thirst system.
