# Sensor

Creates a sensor or binary sensor in Home Assistant which can be updated
from this node.

::: warning
_Needs [Custom Integration](https://github.com/zachowj/hass-node-red) installed
in Home Assistant for this node to function_
:::

## Configuration

### Type <Badge text="required"/>

- Type: `string`
- Values `sensor|binary_sensor`
- Default: `sensor`

The state the entity should be updated to

### State <Badge text="required"/>

- Type: `string | number | boolean`

The state the entity should be updated to

### Attributes

- Type: `Object`

Key/Value pair of attributes to update. The key should be a string and value can be a [string | number | boolean | object]

### Home Assistant Config

- Type: `Object`

Configuration options available for the selected entity

### Input Override

- Type: `string`
- Values: `accept | merge | block`

Determine how input values will be handled. When merge is selected the message object values will override the configuration values.

### Resend state and attributes

- Type: `boolean`

When creating the entity in Home Assistant this will also send the last updated state and attributes then node sent to Home Assistant

## Inputs

properties of `msg.payload`

### state

- Type: `string | number | boolean`

The state the entity should be updated to

### attributes

- Type: `Object`

Key/Value pair of attributes to update. The key should be a string and value can be a `[string | number | boolean | object]`

<!-- TODO: outputs -->
