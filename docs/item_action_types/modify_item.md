# Modify Item
[Item Action Types](../item_action_types.md)

Applies an item modifier to the item stack with a player fulfilling the "this" criteria. The player is currently random.

Type ID: `ra_additions:modify_item`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `modifier` | [Identifier](../data_types/identifier.md) | _optional_ | The Identifier of an item modifier. | 

### Example
```json
{
  "type": "ra_additions:modify_item",
  "modifier": "ra_additions:set_name"
}
```
This example will apply the `ra_additions:set_name` item modifier to the item.
