# Core Settings

The Core Settings section is found under the # CORE SETTINGS line at the top of file.

**`require_perms`:**

The `require_perms` setting decides whether or not players will need permission to use commands and actions for the plugin.

This setting has two options:

`true`

`false`

When set to `true` (which is the default setting), players will need to have the individual permissions to allow them to interact with the plugin.

When set to `false`, players will not need any permissions. Setting this option to `false` is useful if you do not have (and do not want) a permissions plugin, such as LuckPerms.

**`disable_in_worlds`:**

The `disabled_in_worlds` setting is used to stop UndeadPandemic from working in specified worlds. This is ideal if you are using different worlds for different plugins or game modes.

This option uses a string list to specify world names, and each world name should be surrounded by apostrophes, for example, 'world'.
