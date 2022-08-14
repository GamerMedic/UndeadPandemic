# safeZoneData.yml

{% hint style="success" %}
The safeZoneData.yml is a storage file.
{% endhint %}

This file stores the number of plots that a player currently has to create a safezone.

SafeZones are given as a WorldGuard protected chunk, and each player is given 4 by default. The default number cannot be changed, but the number of chunks each player has can be changed using the [`/safezone` command](../commands/safezone/) or by directly editing the safeZoneData.yml file.

{% hint style="warning" %}
**UUIDS**: You will notice that this file uses player UUIDS instead of display names, this is because WorldGuard offers unique protection based on UUIDS.

Player display names are not currently stored in this file, but this will be added in the future.

In the meantime, you can use [this resource](https://mcuuid.net/) to find out what a player's UUID is, so that you can alter this file accurately.
{% endhint %}

The file will look like the file below.

```
a1b2c345-678d-901e-f234-5gh678h90123:
  SafeZone_Blocks: 4
```

{% hint style="warning" %}
_**FUTURE UPDATES**_: This file may be converted into a JSON storage file in a future update.&#x20;

The data contained in this file will be converted automatically.
{% endhint %}
