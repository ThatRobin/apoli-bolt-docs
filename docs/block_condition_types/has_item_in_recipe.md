# Has Item In Recipe
[Block Condition Types](../block_condition_types.md)

Checks if the recipe that outputs this block, has an item in it that matches this condition.

Type ID: `ra_additions:has_item_in_recipe`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `recipe_type` | [Recipe Type](../data_types/recipe_type.md) | _optional_ | The type of recipe to search for, possible values: `crafting`, `smelting`, `blasting`, `smoking`, `campfire_cooking`, `stonecutting` and `smithing` | 
 | `item_condition` | [Item Condition](../item_condition_types.md) | _optional_ | The condition used to check against the input items of the recipe | 

### Example
```json
{
  "type": "ra_additions:has_item_in_recipe",
  "recipe_type": "smelting",
  "item_condition": {
    "type": "ra_additions:is_block"
  }
}
```
This example will check if the smelting recipe to create this block, is also a block
