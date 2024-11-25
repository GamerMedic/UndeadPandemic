# ☣️ Zombie Infections

When a zombie attacks - or a player eats [`Rotten Flesh`](../../items/rotten-flesh.md) - a player there is a chance (set in the [config.yml](../../configuration/legacy-config.yml/) file, or 40% by default) that the player will be infected with the zombie virus.

Being infected causes the following symptoms:

* Poisoned
* Pain
* Lethargy
* Increase appetite
* Weakness
* Confusion

These symptoms can be changed in the [config.yml file](../../configuration/legacy-config.yml/), but if no symptoms exist then the above symptoms will take effect.

These symptoms will last for 2 minutes by default, but this can also be set in the settings.

Pain will cause harm to the player so the player will die if they cannot treat the symptoms before they lose their health.

By default, infections cannot be cured with milk, which is the default vanilla format. This can be changed in the [config.yml file](../../configuration/legacy-config.yml/). Infections can be cured using antibiotics.
