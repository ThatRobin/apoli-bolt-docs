# Evaluate Condition
[Block Condition Types](../block_condition_types.md)

Evaluates a block condition that is stored in a file.

Type ID: `ra_additions:evaluate_condition`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `block_condition` | [String](../data_types/string.md) | _optional_ | The Identifier of the tag or condition file to be evaluated | 

### Example
```json
{
  "type": "ra_additions:evaluate_condition",
  "block_condition": "test_pack:test_condition"
}
```
This example will check the `test_pack:test_condition` block condition.
