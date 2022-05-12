---
description: extends Base
---

# ApplicationCommand

## Constructor

| PARAMETER | TYPE                      | OPTIONAL | DESCRIPTION                     |
| --------- | ------------------------- | -------- | ------------------------------- |
| client    | Client                    | none     | The discord.js client           |
| data      | RawApplicationCommandData | none     | The application command data    |
| manager   | ApplicationCommandManager | none     | The application command manager |

## Properties

### .client

The discord.js client

Type: Client

### .id

The id of the command

Type: Snowflake

### .name

The name of the command

Type: string

### .guildId

The guild id of the command

Type: Snowflake | null

### .applicationId

The application id of the command

Type: Snowflake

### .permissions

The permissions of the command

Type: number

### .description

The description of the command

Type: string | null

### .descriptionLocalizations

The description localizations of the command

Type: { \[locale: string]: string }

### .nameLocalizations

The name localizations of the command

Type: { \[locale: string]: string }

### .global

The global mode of the command

Type: boolean

### .type

The type of the command

Type: { \[locale: string]: string }

### .version

The api version of the command

Type: string

### .options

The options of the command

Type: ApplicationCommandOptionData\[]

### .manager

The application command manager

Type: ApplicationCommandManager

## Methods

### .createdTimestamp

The created timestamp for command

Returns: number

### .createdAt

The created date for command

Returns: Date

### .guild

The guild for command

Returns: Guild | null

### .fetchGuild()

Fetch the guild of command

Returns: Promise\<Guild | null>

### .delete()

Delete the command

Returns: Promise\<void>

### .edit(data)

Edit the command

| PARAMETER | TYPE                       | OPTIONAL | DESCRIPTION          |
| --------- | -------------------------- | -------- | -------------------- |
| data      | ApplicationCommandEditData | none     | New data for command |

Returns: Promise\<ApplicationCommand>

### .fetch()

Fetch the command

Returns: Promise\<ApplicationCommand>

### .setName(name)

Set the name of command

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION         |
| --------- | ------ | -------- | ------------------- |
| name      | string | none     | New name of command |

Returns: Promise\<ApplicationCommand>

### .setNameLocalizations(localizations)

Set the name localizations of command

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                       |
| ------------- | ----------------------------- | -------- | --------------------------------- |
| localizations | { \[locale: string]: string } | none     | New name localizations of command |

Returns: Promise\<ApplicationCommand>

### .setDescription(description)

Set the description of command

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION                |
| ----------- | ------ | -------- | -------------------------- |
| description | string | none     | New description of command |

Returns: Promise\<ApplicationCommand>

### .setDescriptionLocalizations(localizations)

Set the description localizations of command

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                  |
| ------------- | ----------------------------- | -------- | ---------------------------- |
| localizations | { \[locale: string]: string } | none     | New localizations of command |

Returns: Promise\<ApplicationCommand>

### .setOptions(options)

Set the options of command

| PARAMETER | TYPE                            | OPTIONAL | DESCRIPTION            |
| --------- | ------------------------------- | -------- | ---------------------- |
| options   | ApplicationCommandOptionData\[] | none     | New options of command |

Returns: Promise\<ApplicationCommand>

### .setPermissions(permissions)

Set the permissions of command

| PARAMETER   | TYPE                          | OPTIONAL | DESCRIPTION                |
| ----------- | ----------------------------- | -------- | -------------------------- |
| permissions | Permissions \| Permissions\[] | none     | New permissions of command |

Returns: Promise\<ApplicationCommand>

### .setGlobal(global)

Set the global mode of command

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION                |
| --------- | ------- | -------- | -------------------------- |
| global    | boolean | none     | New global mode of command |

Returns: Promise\<ApplicationCommand>

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
