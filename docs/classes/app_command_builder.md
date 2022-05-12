---
description: extends Base
---

# ApplicationCommandBuilder

## Properties

### .name

The command name

Type: string | null

### .guild\_id

The guild id of command

Type: Snowflake | null

### .default\_member\_permissions

The command permissions

Type: string

### .description

The command description

Type: string | null

### .description\_localizations

The command description localizations

Type: { \[locale: string]: string }

### .name\_localizations

The command name localizations

Type: { \[locale: string]: string }

### .dm\_permission

The command global mode

Type: boolean

### .type

The command type

Type: number

### .options

The command options

Type: RawApplicationCommandOptionData\[]

## Methods

### .setName(name)

Set the command name

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION      |
| --------- | ------ | -------- | ---------------- |
| name      | string | none     | The command name |

Returns: ApplicationCommandBuilder

### .setGuildId(guildId)

Set the guild id of command

| PARAMETER | TYPE      | OPTIONAL | DESCRIPTION             |
| --------- | --------- | -------- | ----------------------- |
| guildId   | Snowflake | none     | The guild id of command |

Returns: ApplicationCommandBuilder

### .setPermissions(permissions)

Set the command permissions

| PARAMETER | TYPE                          | OPTIONAL | DESCRIPTION             |
| --------- | ----------------------------- | -------- | ----------------------- |
| name      | Permissions \| Permissions\[] | none     | The command permissions |

Returns: ApplicationCommandBuilder

### .setDescription(description)

Set the command description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION             |
| ----------- | ------ | -------- | ----------------------- |
| description | string | none     | The command description |

Returns: ApplicationCommandBuilder

### .setDescriptionLocalizations(localizations)

Set the command description

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                           |
| ------------- | ----------------------------- | -------- | ------------------------------------- |
| localizations | { \[locale: string]: string } | none     | The command description localizations |

Returns: ApplicationCommandBuilder

### .setNameLocalizations(localizations)

Set the command description

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                    |
| ------------- | ----------------------------- | -------- | ------------------------------ |
| localizations | { \[locale: string]: string } | none     | The command name localizations |

Returns: ApplicationCommandBuilder

### .setGlobal(global)

Set the command global

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION        |
| --------- | ------- | -------- | ------------------ |
| global    | boolean | none     | The command global |

Returns: ApplicationCommandBuilder

### .setType(type)

Set the command type

| PARAMETER | TYPE                    | OPTIONAL | DESCRIPTION      |
| --------- | ----------------------- | -------- | ---------------- |
| type      | ApplicationCommandTypes | none     | The command type |

Returns: ApplicationCommandBuilder

### .addUserOption(fn)

Add the user option

| PARAMETER | TYPE                                 | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------ | -------- | ----------------------------------------- |
| fn        | (builder: UserOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addSubcommandOption(fn)

Add the subcommand option

| PARAMETER | TYPE                                       | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------ | -------- | ----------------------------------------- |
| fn        | (builder: SubcommandOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addSubcommandGroupOption(fn)

Add the subcommand group option

| PARAMETER | TYPE                                            | OPTIONAL | DESCRIPTION                               |
| --------- | ----------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: SubcommandGroupOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addStringOption(fn)

Add the string option

| PARAMETER | TYPE                                   | OPTIONAL | DESCRIPTION                               |
| --------- | -------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: StringOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addIntegerOption(fn)

Add the integer option

| PARAMETER | TYPE                                    | OPTIONAL | DESCRIPTION                               |
| --------- | --------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: IntegerOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addBooleanOption(fn)

Add the boolean option

| PARAMETER | TYPE                                    | OPTIONAL | DESCRIPTION                               |
| --------- | --------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: BooleanOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addChannelOption(fn)

Add the channel option

| PARAMETER | TYPE                                    | OPTIONAL | DESCRIPTION                               |
| --------- | --------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: ChannelOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addRoleOption(fn)

Add the role option

| PARAMETER | TYPE                                 | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------ | -------- | ----------------------------------------- |
| fn        | (builder: RoleOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addMentionableOption(fn)

Add the mentionable option

| PARAMETER | TYPE                                        | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: MentionableOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addNumberOption(fn)

Add the number option

| PARAMETER | TYPE                                   | OPTIONAL | DESCRIPTION                               |
| --------- | -------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: NumberOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .addAttachmentOption(fn)

Add the attachment option

| PARAMETER | TYPE                                       | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------------ | -------- | ----------------------------------------- |
| fn        | (builder: AttachmentOptionBuilder) => void | none     | A function that returns an option builder |

Returns: ApplicationCommandBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
