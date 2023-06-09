---
description: What are Safe Zones, and how do they work?
---

# 🏠 Safe Zones

### What is a Safe Zone?

Safe Zones are a collection of plots where Zombies will not spawn.

#### What are plots?

Plots are equal to one Minecraft chunk (x1 16x16 block extending from Bedrock to the Ceiling (build limit).

### How do Safe Zones work?

Players can create a safe zone by building a plot, or a collection of plots adjacent to each other, which is achieved by using the [`safezone:build` command](../commands/safezone/build.md).

A Safe Zone does not allow Zombies to spawn within its borders.&#x20;

Other players cannot destroy blocks that are protected by Safe Zones.

Safe Zones can be dismantled by using the [safezone:destroy command](../commands/safezone/destroy.md).

### How do you get plots?

Players with admin permissions can use the[ safezone:plots command](../commands/safezone/plots.md) to give or take plots to and from players.

Server admins can also choose to give plots in other ways, as rewards, or as token currency. This is recommended, but at the discretion of admins.

[CraftBook](https://www.spigotmc.org/resources/craftbook.2083/) is recommended to use plots as tokens.

### Are plots protected from players?

In older versions of the plugin, you will need to change the flags in the `config.yml` file. The newest version will prevent other players from opening doors, however, chests are not protected by default.

{% hint style="danger" %}
### Cautions

It's best not to use Safe Zones if you are using a plugin such as Towny or Factions, because the plot protection may conflict with those plugins. The Safe Zone feature is designed to be used as a standalone plot protection system so its use it optional when using other protection plugins.
{% endhint %}

