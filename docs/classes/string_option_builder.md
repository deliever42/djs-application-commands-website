---
description: extends BaseOptionBuilder
---

# StringOptionBuilder

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

### .autocomplete

The option autocomplete

Type: boolean

### .choices

The option choices

Type: RawApplicationCommandOptionChoiceData\[]

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

Returns: StringOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: StringOptionBuilder

### .setRequired(required)

Set the option required

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION         |
| --------- | ------- | -------- | ------------------- |
| required  | boolean | none     | The option required |

Returns: StringOptionBuilder

### .setAutocomplete(autocomplete)

Set the option required

| PARAMETER    | TYPE    | OPTIONAL | DESCRIPTION             |
| ------------ | ------- | -------- | ----------------------- |
| autocomplete | boolean | none     | The option autocomplete |

Returns: StringOptionBuilder

### .addChoice(choice)

Add the option choice

| PARAMETER | TYPE                                 | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------ | -------- | ----------------------------------------- |
| choice    | fn: (builder: ChoiceBuilder) => void | none     | A function that returns an option builder |

Returns: StringOptionBuilder

### .addChoices(...choices)

Add the option choices

| PARAMETER  | TYPE                                  | OPTIONAL | DESCRIPTION                               |
| ---------- | ------------------------------------- | -------- | ----------------------------------------- |
| ...choices | ((builder: ChoiceBuilder) => void)\[] | none     | A function that returns an option builder |

Returns: StringOptionBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
