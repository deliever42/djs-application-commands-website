---
description: extends Base
---

# ChoiceBuilder

## Properties

### .name

The choice name

Type: string | null

### .name\_localizations

The choice name localizations

Type: { \[locale: string]: string }

### .value

The choice value

Type: string | number

## Methods

### .setName(name)

Set the choice name

| PARAMETER | TYPE   | OPTIONAL | DESCRIPTION     |
| --------- | ------ | -------- | --------------- |
| name      | string | none     | The choice name |

Returns: ChoiceBuilder

### .setValue(value)

Set the choice value

| PARAMETER | TYPE             | OPTIONAL | DESCRIPTION      |
| --------- | ---------------- | -------- | ---------------- |
| value     | string \| number | none     | The choice value |

Returns: ChoiceBuilder

### .setNameLocalizations(localizations)

Set the choice name localizations

| PARAMETER     | TYPE                          | OPTIONAL | DESCRIPTION                   |
| ------------- | ----------------------------- | -------- | ----------------------------- |
| localizations | { \[locale: string]: string } | none     | The choice name localizations |

Returns: ChoiceBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
