---
description: extends BaseOption
---

# SubcommandOptionBuilder

## Properties

### .name

The option name

Type: string | null

### .description

The option description

Type: string | null

### .type

The option type

Type: number

### .options

The subcommand options

Type: RawApplicationCommandOptionData\[]

### .name\_localizations

The option name localizations

Type: { \[locale: string]: string }

### .description\_localizations

The option description localizations

Type: { \[locale: string]: string }

## Methods

### .setName(name)

Set the option name

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION     |
| --------- | ------ | -------- | --------------- |
| name      | string | none     | The option name |

Returns: SubcommandOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: SubcommandOptionBuilder

### .addUserOption(fn)

Add the user option

| PARAMETER | TYPE                                              | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: UserOptionBuilder) => UserOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addStringOption(fn)

Add the string option

| PARAMETER | TYPE                                                  | OPTIONAL | DESCRIPTION                               |
| --------- | ----------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: StringOptionBuilder) => StringOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addIntegerOption(fn)

Add the integer option

| PARAMETER | TYPE                                                    | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: IntegerOptionBuilder) => IntegerOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addBooleanOption(fn)

Add the boolean option

| PARAMETER | TYPE                                                    | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: BooleanOptionBuilder) => BooleanOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addChannelOption(fn)

Add the channel option

| PARAMETER | TYPE                                                    | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: ChannelOptionBuilder) => ChannelOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addRoleOption(fn)

Add the role option

| PARAMETER | TYPE                                              | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: RoleOptionBuilder) => RoleOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addMentionableOption(fn)

Add the mentionable option

| PARAMETER | TYPE                                                            | OPTIONAL | DESCRIPTION                               |
| --------- | --------------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: MentionableOptionBuilder) => MentionableOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addNumberOption(fn)

Add the number option

| PARAMETER | TYPE                                                  | OPTIONAL | DESCRIPTION                               |
| --------- | ----------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: NumberOptionBuilder) => NumberOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .addAttachmentOption(fn)

Add the attachment option

| PARAMETER | TYPE                                                          | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: AttachmentOptionBuilder) => AttachmentOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandOptionBuilder

### .setNameLocalizations(localizations)

Set the option name localizations

| PARAMETER     | TYPE                           | OPTIONAL | DESCRIPTION                   |
| ------------- | ------------------------------ | -------- | ----------------------------- |
| localizations | s{ \[locale: string]: string } | none     | The option name localizations |

Returns: SubcommandGroupOptionBuilder

### .setDescriptionLocalizations(localizations)

Set the option description localizations

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                          |
| ------------- | ----------------------------- | -------- | ------------------------------------ |
| localizations | { \[locale: string]: string } | none     | The option description localizations |

Returns: SubcommandGroupOptionBuilder
