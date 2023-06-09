# Health Settings

These settings will determine what items are used as the three health restoring items.

1. _Adrenaline_
2. _Antibiotics_
3. _Bandage_
4. _First Aid Kit_

Each item has the same set up:

**`itemName`**:

This is the ID of the item.

**`name`**:

This is the name of the item, this can be anything you want.

{% hint style="info" %}
_**TIP**_: Minecraft colours can be used in the item name and lore.
{% endhint %}

**`lore`**:

This is the lore for the item, again, this can be anything you want.

**`material`**:

This is the Minecraft material that you want to use for the item.

{% hint style="danger" %}
**material** is not a valid configuration setting for `first_aid_kit`, which will always be set as a chest.

If you try to set this option, it will just be ignored.
{% endhint %}

**`data`**:

Data sets the custom model data for the item. You can set this to whatever you want, but it will need to correspond to your resource pack. If you have not set up your own resource pack, then you can use the UndeadPandemic resource pack. Items will be already be set up to work with the config.

#### Here is an example item.

```yaml
adrenaline:
  name: 'Adrenaline'
  lore: 'Temporarily Cure an Infection'
  material: MUSIC_DISC_MALL
  data: 123456
```
