# RawApplicationCommandOptionData

### Type: Object\<string, any>

### Properties

| PARAMETER                  | TYPE                                     | DESCRIPTION                              |
| -------------------------- | ---------------------------------------- | ---------------------------------------- |
| type                       | number                                   | The option type                          |
| name                       | string                                   | The option name                          |
| name\_localizations        | { \[locale: string]: string }            | The option name localizations            |
| description                | string                                   | The option description                   |
| description\_localizations | { \[locale: string]: string }            | The option and description localizations |
| required                   | boolean                                  | The option required                      |
| choices                    | RawApplicationCommandOptionChoiceData\[] | The option chocies                       |
| options                    | RawApplicationCommandOptionData\[]       | The option option                        |
| channel\_types             | number\[]                                | The option name                          |
| min\_value                 | number                                   | The option min value                     |
| max\_value                 | number                                   | The option max value                     |
| autocomplete               | boolean                                  | The option autocomplete                  |

See also: [https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-option-structure](https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-option-structure)
