# Zombie Settings

Zombie settings determine chance of zombies spawning, as well the rate that they spawn, and whether zombies are attracted by gun fire.

**`zombie_spawn_rate`**:

The rate at which zombies will spawn during the night. This is set to `5` by default. This can be any integer.

Disable the spawn rate by setting this value to `-1`. Disabling the spawn right doesn't prevent zombies from spawning, it only restricts the zombie spawn rates to the vanilla settings.

{% hint style="danger" %}
The higher that the spawn rate is the slower that your server will be. So unless you have a supercomputer as your Minecraft server, do not set this rate above 10.
{% endhint %}

**`attract_zombie_rate`**:

This rate will determine how many zombies spawn when a loud weapon is used. This defaults to `2`. Same rules apply as the **`zombie_spawn_rate`**; don't set this rate above 10.

**`attract_zombie_radius`**:

This radius will determine how far away (in blocks) zombies will spawn when a loud weapon is used.

This defaults to `5` but for realism it is recommended to set this to at least `7`. Just bear in mind that the higher the radius, the higher the CPU load, especially when combined with a higher **`attract_zombie_rate`**.

**`attract_zombie_chance`**:

This is the percentage chance that zombies will be attracted to the sound of loud weapons. This is set to `70%` by default. This setting must be between 0 and 100, you can set it as any number but the plugin will ignore the abnormal setting. Instead, if this is set above 100 then the chance will be set to 100%, and below 0 the chance will be set to 0%.
