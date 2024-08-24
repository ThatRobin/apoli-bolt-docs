# Execute Action
[Block Action Types](../block_action_types.md)

Executes a block action that is stored in a file.

Type ID: `ra_additions:execute_action`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `block_action` | [String](../data_types/string.md) | _optional_ | The Identifier of the tag or action file to be executed | 

### Example
```json
{
  "type": "ra_additions:execute_action",
  "block_action": "ra_additions:add_block"
}
```
This example will run the `ra_additions:add_block` block action.
