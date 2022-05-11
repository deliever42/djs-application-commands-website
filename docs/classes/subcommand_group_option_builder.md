---
description: extends BaseOption
---

# SubcommandGroupOptionBuilder

## Properties

### .name

The option name

Type: string | null

### .type

The option type

Type: number

### .options

The subcommand group options

Type: RawApplicationCommandOptionData\[]

## Methods

### .setName(name)

Set the option name

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION     |
| --------- | ------ | -------- | --------------- |
| name      | string | none     | The option name |

Returns: SubcommandGroupOptionBuilder

### .addSubcommandOption(fn)

Add the subcommand option

| PARAMETER | TYPE                                                           | OPTIONAL | DESCRIPTION                               |
| --------- | -------------------------------------------------------------- | -------- | ----------------------------------------- |
| fn        | (builder: SSubcommandOptionBuilder) => SubcommandOptionBuilder | none     | A function that returns an option builder |

Returns: SubcommandGroupOptionBuilder
