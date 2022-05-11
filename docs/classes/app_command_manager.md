---
description: extends CachedManager<Snowflake, ApplicationCommand>
---

# ApplicationCommandManager

## Properties

### .client

The discord.js client

Type: Client

### .rest

The rest api

Type: REST

### .cache

The cache of application commands

Type: Collection\<Snowflake, ApplicationCommand>

## Methods

### .set(commands, guildId)

Set the commands

| PARAMETER | TYPE                      | OPTIONAL | DESCRIPTION                                         |
| --------- | ------------------------- | -------- | --------------------------------------------------- |
| commands  | ApplicationCommandData\[] | none     | Command datas to set commands                       |
| guildId   | Snowflake                 | yes      | The id of the server where the commands will be set |

Returns: Promise\<Collection\<Snowflake, ApplicationCommand>>

### .create(command, guildId)

Create the command

| PARAMETER | TYPE                   | OPTIONAL | DESCRIPTION                                        |
| --------- | ---------------------- | -------- | -------------------------------------------------- |
| command   | ApplicationCommandData | none     | Command data to set command                        |
| guildId   | Snowflake              | yes      | The id of the server where the command will be set |

Returns: Promise\<ApplicationCommand>

### .delete(commandId, guildId)

Delete the command

| PARAMETER | TYPE      | OPTIONAL | DESCRIPTION                                           |
| --------- | --------- | -------- | ----------------------------------------------------- |
| commandId | Snowflake | none     | Command id to delete command                          |
| guildId   | Snowflake | yes      | The id of the server where the command will be delete |

Returns: Promise\<void>

### .edit(commandId, data, guildId)

Edit the command

| PARAMETER | TYPE                       | OPTIONAL | DESCRIPTION                                         |
| --------- | -------------------------- | -------- | --------------------------------------------------- |
| commandId | Snowflake                  | none     | Command id to edit command                          |
| data      | ApplicationCommandEditData | none     | New data to edit command                            |
| guildId   | Snowflake                  | yes      | The id of the server where the command will be edit |

Returns: Promise\<ApplicationCommand>

### .fetch(commandId, guildId)

Fetch the command

| PARAMETER | TYPE      | OPTIONAL | DESCRIPTION                                          |
| --------- | --------- | -------- | ---------------------------------------------------- |
| commandId | Snowflake | none     | Command id to fetch command                          |
| guildId   | Snowflake | yes      | The id of the server where the command will be fetch |

Returns: Promise\<ApplicationCommand>

### .setName(commandId, name, guildId)

Set the name of command

|           | TYPE      | OPTIONAL | DESCRIPTION         |
| --------- | --------- | -------- | ------------------- |
| commandId | Snowflake | none     | The command id      |
| name      | string    | none     | New name of command |
| guildId   | boolean   | yes      | Guild id of command |

Returns: Promise\<ApplicationCommand>

### .setNameLocalizations(commandId, localizations, guildId)

Set the name localizations of command

|               | TYPE                          | OPTIONAL | DESCRIPTION                       |
| ------------- | ----------------------------- | -------- | --------------------------------- |
| commandId     | Snowflake                     | none     | The command id                    |
| localizations | { \[locale: string]: string } | none     | New name localizations of command |
| guildId       | boolean                       | yes      | Guild id of command               |

Returns: Promise\<ApplicationCommand>

### .setDescription(commandId, description, guildId)

Set the description of command

|             | TYPE      | OPTIONAL | DESCRIPTION                |
| ----------- | --------- | -------- | -------------------------- |
| commandId   | Snowflake | none     | The command id             |
| description | string    | none     | New description of command |
| guildId     | boolean   | yes      | Guild id of command        |

Returns: Promise\<ApplicationCommand>

### .setDescriptionLocalizations(commandId, localizations, guildId)

Set the description localizations of command

|               | TYPE                          | OPTIONAL | DESCRIPTION                              |
| ------------- | ----------------------------- | -------- | ---------------------------------------- |
| commandId     | Snowflake                     | none     | The command id                           |
| localizations | { \[locale: string]: string } | none     | New description localizations of command |
| guildId       | boolean                       | yes      | Guild id of command                      |

Returns: Promise\<ApplicationCommand>

### .setOptions(commandId, options, guildId)

Set the options of command

|           | TYPE                            | OPTIONAL | DESCRIPTION            |
| --------- | ------------------------------- | -------- | ---------------------- |
| commandId | Snowflake                       | none     | The command id         |
| options   | ApplicationCommandOptionData\[] | none     | New options of command |
| guildId   | boolean                         | yes      | Guild id of command    |

Returns: Promise\<ApplicationCommand>

### .setPermissions(commandId, permissions, guildId)

Set the permissions of command

|             | TYPE                          | OPTIONAL | DESCRIPTION                |
| ----------- | ----------------------------- | -------- | -------------------------- |
| commandId   | Snowflake                     | none     | The command id             |
| permissions | Permissions \| Permissions\[] | none     | New permissions of command |
| guildId     | boolean                       | yes      | Guild id of command        |

Returns: Promise\<ApplicationCommand>

### .setGlobal(commandId, global, guildId)

Set the global mode of command

|           | TYPE      | OPTIONAL | DESCRIPTION                |
| --------- | --------- | -------- | -------------------------- |
| commandId | Snowflake | none     | The command id             |
| global    | boolean   | none     | New global mode of command |
| guildId   | boolean   | yes      | Guild id of command        |

Returns: Promise\<ApplicationCommand>
