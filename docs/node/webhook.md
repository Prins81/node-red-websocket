# Webhook

Outputs the data received from the created webhook in Home Assistant

::: warning
_Needs [Custom Integration](https://github.com/zachowj/hass-node-red) installed
in Home Assistant for this node to function_
:::

## Configuration

### ID <Badge text="required"/>

- Type: `string`

A string to be used for the webhook URL in Home Assistant.

### Allowed Methods <Badge text="required"/>

- Type: `list`

A list of allowed methods that Home Assistant will accept for the webhook. At least one method must be selected.

## Outputs

Value types:

- `received data`: The parsed body from the webhook request
- `trigger id`: webhook id
- `headers`: entity state of the triggered entity
- `params`: Query string parameters
- `config`: config properties of the node
