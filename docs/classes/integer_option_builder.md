---
description: extends BaseOptionBuilder
---

# IntegerOptionBuilder

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

### .max\_value

The option max value

Type: number | null

### .min\_value

The option min value

Type: number | null

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

Returns: IntegerOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: IntegerOptionBuilder

### .setRequired(required)

Set the option required

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION         |
| --------- | ------- | -------- | ------------------- |
| required  | boolean | none     | The option required |

Returns: IntegerOptionBuilder

### .setAutocomplete(autocomplete)

Set the option required

| PARAMETER    | TYPE    | OPTIONAL | DESCRIPTION             |
| ------------ | ------- | -------- | ----------------------- |
| autocomplete | boolean | none     | The option autocomplete |

Returns: IntegerOptionBuilder

### .addChoice(choice)

Add the option choice

| PARAMETER | TYPE                                 | OPTIONAL | DESCRIPTION                               |
| --------- | ------------------------------------ | -------- | ----------------------------------------- |
| choice    | fn: (builder: ChoiceBuilder) => void | none     | A function that returns an option builder |

Returns: IntegerOptionBuilder

### .addChoices(...choices)

Add the option choices

| PARAMETER  | TYPE                                  | OPTIONAL | DESCRIPTION                               |
| ---------- | ------------------------------------- | -------- | ----------------------------------------- |
| ...choices | ((builder: ChoiceBuilder) => void)\[] | none     | A function that returns an option builder |

Returns: IntegerOptionBuilder

### .setMaxValue(maxValue)

Set the option max value

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION          |
| --------- | ------ | -------- | -------------------- |
| maxValue  | number | none     | The option max value |

Returns: IntegerOptionBuilder

### .setMinValue(minValue)

Set the option min value

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION          |
| --------- | ------ | -------- | -------------------- |
| minValue  | number | none     | The option min value |

Returns: IntegerOptionBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
