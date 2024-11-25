# /keycard (Legacy)

{% hint style="danger" %}
This command was removed in v3.0.0.
{% endhint %}

![Key Card Texture](../.gitbook/assets/keycard.png)

### Command Structure

`<required parameter>`

`[optional parameter]`

`/keycard`<mark style="color:purple;">`<cut>`</mark> <mark style="color:orange;">`<X co-ordinate>`</mark> <mark style="color:orange;">`<Y co-ordinate> <Z co-ordinate>`</mark> <mark style="color:red;">`[keycard description]`</mark> <mark style="color:yellow;">`[uses]`</mark> <mark style="color:green;">`[quantity]`</mark>

![](../.gitbook/assets/keycard_cmd.png)

### Parameter Descriptions

_**Co-Ordinates**_

The X, Y, Z co-ordinates are the co-ordinates of the door that you'd like the key card to open.

{% hint style="info" %}
_**PRO TIP**_: If you use tildes (\~) in place of numeric co-ordinates, the key card will use your current location.

Using +/- after the tildes will offset your location by the amount you specify. For example, if your co-ordinates are 100 70 200, \~ \~ \~ will equal 100 70 200; and \~+10 \~ \~-20 will equal 110 70 180.
{% endhint %}

A door must be placed on the co-ordinates that you set the key card to, otherwise the key card will be useless.

_**Keycard Description**_

The keycard decription is the lore of the key card item. If you do not set the description, the lore will default to the keycard lore set in config.yml.

You cannot use spaces in the description, instead, replace spaces with an underscore ( \_ ).

You can add new lines to the key lore by adding a pipe ( | ) to the key card description.

{% hint style="success" %}
Example:

`/keycard cut ~ ~ ~+1 This_key_will_open|a_special_door! 5`
{% endhint %}

_**Uses**_

This is the number of uses that the player will be allowed to have before the key card is 'used' (removed from their inventory).

If this is not set, then the key card will only be used once.

{% hint style="danger" %}
If the **keycard description** parameter is not set, then you cannot set this value. You will have to provide a **keycard description** to use this parameter.
{% endhint %}

**Quantity**

The quantity parameter determines how many key cards the player will be given. All of the key cards given will have the same values (so will open the same door).
