# Using Translations

### Enabling Language Support

The plugin has multilingual support which can be utilised by changing the defined language in the config.yml file.

In the default config.yml file the `language` parameter is near the top of the file, but if missing can be added anywhere.

### Defining the Desired Language

The UndeadPandemic plugin utilises ISO 639-1 standard language codes ([you can find a list here](https://en.wikipedia.org/wiki/List\_of\_ISO\_639-1\_codes) - use the 639-1 column).

Not many languages are currently supported by the plugin as of _08/10/2022_.

### Support Languages

A list of currently supported languages:

|      Language      | Language Code |
| :----------------: | :-----------: |
|  (British) English |       en      |
|  (Deutsch) German  |       de      |
| (Nederlands) Dutch |       nl      |
|  (Français) French |       fr      |

### Editing Language Files

You can freely edit the desired language files. Use of Minecraft colour codes is supported in language files. [Click here to view a Minecraft Colour Codes list](https://minecraftitemids.com/color-codes).

The standard usage for colours code within the plugin is: `&{colourCode}` . Example: `&4`.

_<mark style="color:yellow;">Do not</mark>_ edit any variable names because the variable will not work if changed.

**Example of a variable:**

```yaml
{player}
```

#### Contributors

The French language file was translated by Minecraft Player Lucachinou
