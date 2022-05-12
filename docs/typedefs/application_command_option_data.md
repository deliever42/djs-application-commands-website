# ApplicationCommandOptionData

### Type: Object\<string, any>

### Properties

| PARAMETER                | TYPE                                  | DESCRIPTION                          |
| ------------------------ | ------------------------------------- | ------------------------------------ |
| name                     | string                                | The option name                      |
| type                     | ApplicationCommandOptionTypes         | The option type                      |
| nameLocalizations        | { \[locale: string]: string }         | The option name localizations        |
| description              | string                                | The option description               |
| descriptionLocalizations | { \[locale: string]: string }         | The option description localizations |
| required                 | boolean                               | The option required                  |
| choices                  | ApplicationCommandOptionChoiceData\[] | The option choices                   |
| options                  | ApplicationCommandOptionData\[]       | The subcommand options               |
| channelTypes             | ChannelTypes\[]                       | The option channel types             |
| minValue                 | number                                | The option min value                 |
| maxValue                 | number                                | The option max value                 |
| autocomplete             | boolean                               | The option autocomplete              |
