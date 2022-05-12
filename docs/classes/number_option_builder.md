---
description: extends BaseOption
---

# NumberOptionBuilder

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

Returns: NumberOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: NumberOptionBuilder

### .setRequired(required)

Set the option required

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION         |
| --------- | ------- | -------- | ------------------- |
| required  | boolean | none     | The option required |

Returns: NumberOptionBuilder

### .setAutocomplete(autocomplete)

Set the option required

| PARAMETER    | TYPE    | OPTIONAL | DESCRIPTION             |
| ------------ | ------- | -------- | ----------------------- |
| autocomplete | boolean | none     | The option autocomplete |

Returns: NumberOptionBuilder

### .addChoice(choice)

Add the option choice

| PARAMETER | TYPE                               | OPTIONAL | DESCRIPTION       |
| --------- | ---------------------------------- | -------- | ----------------- |
| choice    | ApplicationCommandOptionChoiceData | none     | The option choice |

Returns: NumberOptionBuilder

### .addChoices(...choices)

Add the option choices

| PARAMETER  | TYPE                                  | OPTIONAL | DESCRIPTION        |
| ---------- | ------------------------------------- | -------- | ------------------ |
| ...choices | ApplicationCommandOptionChoiceData\[] | none     | The option choices |

Returns: NumberOptionBuilder

### .setMaxValue(maxValue)

Set the option max value

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION          |
| --------- | ------ | -------- | -------------------- |
| maxValue  | number | none     | The option max value |

Returns: NumberOptionBuilder

### .setMinValue(minValue)

Set the option min value

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION          |
| --------- | ------ | -------- | -------------------- |
| minValue  | number | none     | The option min value |

Returns: NumberOptionBuilder
