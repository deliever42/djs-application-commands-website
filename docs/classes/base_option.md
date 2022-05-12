# BaseOption

## Constructor

| PARAMETER | TYPE                          | OPTIONAL | DESCRIPTION      |
| --------- | ----------------------------- | -------- | ---------------- |
| type      | ApplicationCommandOptionTypes | none     | Type option type |

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

Returns: BaseOption

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: BaseOption

### setNameLocalizations(localizations)

Set the option name localizations

| PARAMETER     | TYPE                           | OPTIONAL | DESCRIPTION                   |
| ------------- | ------------------------------ | -------- | ----------------------------- |
| localizations | s{ \[locale: string]: string } | none     | The option name localizations |

Returns: BaseOption

### setDescriptionLocalizations(localizations)

Set the option description localizations

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                          |
| ------------- | ----------------------------- | -------- | ------------------------------------ |
| localizations | { \[locale: string]: string } | none     | The option description localizations |

Returns: BaseOption
