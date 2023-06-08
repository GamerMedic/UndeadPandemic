---
description: What is the thirst system? And how does it work?
---

# Thirst System

### What is the thirst system?

The thirst system allows players to experience thirst within the game. It is represented by a blue boss bar.

<figure><img src="../../.gitbook/assets/thirst-bar.webp" alt=""><figcaption><p>Thirst Boss Bar</p></figcaption></figure>

### How does the thirst system work?

#### Dehydration

When enabled, the thirst boss bar will be set to 80% by default, and will decrease every x seconds. The rate of dehydration is set by the `dehydration_rate` and the `dehydration_qty` settings.

#### Becoming Unwell

The player will be alerted when they start to become dehydrated. They will get a message when they hit 50% and 25%.

When a player hits 5% thirst, dehydration will start taking effect. The player will become confused and lethargic, altering their state of mind.

#### Rehydration

A player can restore their hydration levels, and become well again, by using consumables. Consumables will replenish their hydration level according to the [Consumables setting](../../configuration/config.yml/thirst-settings.md).

### Consequences

There are no longer any significant consequences for using the thirst system. Previous versions used the XP system to demonstrate thirst, which discouraged the vanilla XP mechanics. This is no longer the case.
