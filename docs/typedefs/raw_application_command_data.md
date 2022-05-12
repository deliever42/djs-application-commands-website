# RawApplicationCommandData

### Type: Object\<string, any>

### Properties

| PARAMETER                    | TYPE                               | DESCRIPTION                           |
| ---------------------------- | ---------------------------------- | ------------------------------------- |
| id                           | Snowflake                          | The command id                        |
| type                         | number                             | The command type                      |
| application\_id              | Snowflake                          | The command application id            |
| guild\_id                    | Snowflake                          | The command guild id                  |
| name                         | string                             | The command name                      |
| name\_localizations          | { \[locale: string]: string }      | The command name localizations        |
| description                  | string                             | The command description               |
| description\_localizations   | { \[locale: string]: string }      | The command description localizations |
| options                      | RawApplicationCommandOptionData\[] | The command options                   |
| default\_member\_permissions | string                             | The command permissions               |
| dm\_permission               | boolean                            | The command global                    |
| version                      | string                             | The api version                       |

See also: [https://discord.com/developers/docs/interactions/application-commands#application-command-object](https://discord.com/developers/docs/interactions/application-commands#application-command-object)
