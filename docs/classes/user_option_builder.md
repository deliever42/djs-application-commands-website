---
description: extends BaseOptionBuilder
---

# UserOptionBuilder

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

### .required

The option required

Type: boolean

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

Returns: UserOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: UserOptionBuilder

### .setRequired(required)

Set the option required

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION         |
| --------- | ------- | -------- | ------------------- |
| required  | boolean | none     | The option required |

Returns: UserOptionBuilder

### .setNameLocalizations(localizations)

Set the option name localizations

| PARAMETER     | TYPE                           | OPTIONAL | DESCRIPTION                   |
| ------------- | ------------------------------ | -------- | ----------------------------- |
| localizations | s{ \[locale: string]: string } | none     | The option name localizations |

Returns: UserOptionBuilder

### .setDescriptionLocalizations(localizations)

Set the option description localizations

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                          |
| ------------- | ----------------------------- | -------- | ------------------------------------ |
| localizations | { \[locale: string]: string } | none     | The option description localizations |

Returns: UserOptionBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
