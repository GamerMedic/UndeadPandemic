---
description: Everything you need to know about Zombies.
---

# 🧟♂ Zombies

You can add an unlimited number of different zombie types.

{% hint style="info" %}
You can enable and disable zombie types in the config. The plugin will default to using vanilla zombies if all zombies are disabled.
{% endhint %}

### Creating a New Type

To create a new type of zombie you just need to [add the configuration settings in config.yml](../../configuration/config.yml/zombie-settings.md).

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden></th><th data-hidden></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td>Strong Zombie</td><td></td><td></td><td><a href="../../.gitbook/assets/strong_zombie.webp">strong_zombie.webp</a></td></tr><tr><td>Stupid Zombie</td><td></td><td></td><td><a href="../../.gitbook/assets/stupid_zombie.webp">stupid_zombie.webp</a></td></tr><tr><td>Hoard</td><td></td><td></td><td><a href="../../.gitbook/assets/hoarde.webp">hoarde.webp</a></td></tr></tbody></table>

### Hordes

Hoards currently rely on spawn rates and are not controllable. But there will be better hoarde functionality introduced into v2.7.0.

In the v2.7.0 update hoards will more orchestrated and more aggressively attack players, no matter what type of zombie. Zombie types in hordes will generate as per the odds set in the [`config.yml`](../../configuration/config.yml/) file.

Hoards will be configuration in the config file and can be timed, or appear at random. And players with permission will also be able to start a hoard using a new command.

### Infections

Zombies have a chance of infecting the player. These minor infections are curable using antibiotics, but the infections will slowly kill the player if left untreated.

{% content-ref url="zombie-infections.md" %}
[zombie-infections.md](zombie-infections.md)
{% endcontent-ref %}

### Attributes

Since v2.5.0 zombies are almost entirely customisable. You can create your own zombies that can be powerful or weak and slow, or stupid.

You can even put your zombies in a suit of armour. Be sure to strike the balance between challenging gameplay and overpowered zombie mutants!

{% content-ref url="zombie-attributes.md" %}
[zombie-attributes.md](zombie-attributes.md)
{% endcontent-ref %}
