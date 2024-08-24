# Use Internal Block
[Entity Action Types](../entity_action_types.md)

Opens the specified choice screen for the player it is executed as.

Type ID: `ra_additions:use_internal_block`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `block_power` | [Power Type](../data_types/power_type.md) | _optional_ | The Identifier of the choice layer that the action will open. | 

### Example
```json
{
  "type": "ra_additions:use_internal_block",
  "block_power": "ra_additions:furnace_example"
}
```

