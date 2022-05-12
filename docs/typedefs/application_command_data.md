# ApplicationCommandData

### Type: Object\<string, any>

### Properties

| PARAMETER                | TYPE                            | DESCRIPTION                           |
| ------------------------ | ------------------------------- | ------------------------------------- |
| name                     | string                          | The command name                      |
| nameLocalizations        | { \[locale: string]: string }   | The command name localizations        |
| description              | string                          | The command description               |
| descriptionLocalizations | { \[locale: string]: string }   | The command description localizations |
| type                     | ApplicationCommandTypes         | The command type                      |
| options                  | ApplicationCommandOptionData\[] | The command options                   |
| permissions              | Permissions \| Permissions\[]   | The command permissions               |
| global                   | boolean                         | The command global                    |
| guildId                  | Snowflake                       | Guild id of command                   |
