# ApplicationCommandEditData

### Type: Object\<string, any>

### Properties

| PARAMETER                | TYPE                            | DESCRIPTION                              |
| ------------------------ | ------------------------------- | ---------------------------------------- |
| name                     | string                          | The new command name                     |
| nameLocalizations        | { \[locale: string]: string }   | The new command name locazalitons        |
| description              | string                          | The new command description              |
| descriptionLocalizations | { \[locale: string]: string }   | The new command description locazalitons |
| type                     | ApplicationCommandTypes         | The new command type                     |
| options                  | ApplicationCommandOptionData\[] | The new command options                  |
| permissions              | Permissions \| Permissions\[]   | The new command permissions              |
| global                   | boolean                         | The new command global                   |
| guildId                  | Snowflake                       | The new command guildId                  |
