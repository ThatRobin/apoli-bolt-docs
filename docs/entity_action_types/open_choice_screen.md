# Open Choice Screen
[Entity Action Types](../entity_action_types.md)

Opens the specified choice screen for the player it is executed as.

Type ID: `ra_additions:open_choice_screen`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `choice_layer` | [Identifier](../data_types/identifier.md) | _optional_ | The Identifier of the choice layer that the action will open. | 

### Example
```json
{
  "type": "ra_additions:open_choice_screen",
  "choice_layer": "ra_additions:choice_layer_example"
}
```
This example will open the choice screen for the `ra_additions:choice_layer_example` layer.
