# Equipped Trinket
[Entity Condition Types](../entity_condition_types.md)

Checks all the players trinket slots with an Item Condition.

This condition type requires the Trinkets mod to be installed in order to function.

Type ID: `ra_additions:equipped_trinket`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `item_condition` | [Item Condition](../item_condition_types.md) | _optional_ | The items that are searched for in the trinket slots. | 

### Example
```json
{
  "type": "ra_additions:equipped_trinket",
  "item_condition": {
    "type": "apoli:ingredient",
    "ingredient": {
      "item": "minecraft:emerald"
    }
  }
}
```
This example will check if the entity has an emerald equipped in any of their trinkets slots.
