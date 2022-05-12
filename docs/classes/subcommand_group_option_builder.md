---
description: extends BaseOptionBuilder
---

# SubcommandGroupOptionBuilder

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

The subcommand group options

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

Returns: SubcommandGroupOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: SubcommandGroupOptionBuilder

### .addSubcommandOption(fn)

Add the subcommand option

| PARAMETER | TYPE                                                           | OPTIONAL | DESCRIPTION                               |
| --------- | -------------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: SSubcommandOptionBuilder) => SubcommandOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandGroupOptionBuilder

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

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
