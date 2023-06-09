---
description: What is the Health System? And how does it work?
---

# 💊 Health System

{% hint style="warning" %}
This page will take effect from v2.6.0. Information on existing systems will not be included on this page until v2.6.0 is released.
{% endhint %}

### What is the Health System?

The health system encompasses the following variables:

* [Thirst](thirst-system.md)
* Illness / Injury

### Health Status

The health status is the players' current level of health. This will either be '<mark style="color:green;">Healthy</mark>' or '<mark style="color:red;">Unhealthy</mark>'. If the player is unhealthy, then the status will display one of the health conditions listed below.

If the health status is unhealthy then the player will have potion effects applied based on the health condition. Some of these effects can be customised, but the default effects are listed below.

|     Condition     |                                                                 Effects                                                                |                                         After Effects                                        |
| :---------------: | :------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------: |
|  Zombie Infection |                                 Poison; Pain (Harm); Lethargy (Slowness); Hunger; Confusion; Weakness;                                 |                             Death if not cured with antibiotics.                             |
|    Dehydration    |                                                         Confusion; Pain (Harm);                                                        |                                Death if not cured by drinking.                               |
|     Starvation    |                                               Hunger; Confusion; Pain (Harm); Blindness;                                               |                                 Death if not cured by eating.                                |
|     Infection     |                                                     Lethargy (Slowness); Weakness;                                                     |                  None. An infection will heal over time or with antibiotics.                 |
|    Broken Bone    |                                                         Slowness; Pain (Harm);                                                         |                   None. A broken bone will heal over time or with a splint.                  |
|    Hypothermia    |                                                     Slowness; Weakness; Pain (Harm)                                                    |                      Death if not cured by drinking soup or warming up.                      |
|     Depression    |                                                           Slowness; Weakness;                                                          |                        Suicide if not treated by exercise or talking.                        |
|       Mania       | Paraesthesia (Damage Resistance & Health Boost);  Strength (Increase Damage); Luck; Radiance (Glowing); Quickness (Speed); Depression; | Mania will go away on its own but it will cause depression. Depression must then be treated. |

### Thirst

{% hint style="danger" %}
Please refer to the [thirst system](../thirst-system-legacy.md) if you are using any version pre-v2.6.0.
{% endhint %}

The thirst system works largely in the same way as it did before, except the players thirst can be displayed in a boss bar or using PAPI placeholders instead of the XP bar.

Previously, player effects were applied based on the level of thirst. From v2.6.0 effects will instead be applied based on the player's health status.
