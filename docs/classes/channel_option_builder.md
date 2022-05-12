---
description: extends BaseOptionBuilder
---

# ChannelOptionBuilder

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

### .channel\_types

Type option channel types

Type: number\[] | null

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

Returns: ChannelOptionBuilder

### .setDescription(description)

Set the option description

| PARAMETER   | TYPE   | OPTIONAL | DESCRIPTION            |
| ----------- | ------ | -------- | ---------------------- |
| description | string | none     | The option description |

Returns: ChannelOptionBuilder

### .setRequired(required)

Set the option required

| PARAMETER | TYPE    | OPTIONAL | DESCRIPTION         |
| --------- | ------- | -------- | ------------------- |
| required  | boolean | none     | The option required |

Returns: ChannelOptionBuilder

### .setChannelTypes(channelTypes)

Set the option channel types

| PARAMETER    | TYPE            | OPTIONAL | DESCRIPTION              |
| ------------ | --------------- | -------- | ------------------------ |
| channelTypes | ChannelTypes\[] | none     | The option channel types |

Returns: ChannelOptionBuilder

### .toJSON()

Returns the properties of the class in the object type.

Returns: { \[property: string]: any }
