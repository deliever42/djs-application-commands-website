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
