# Evaluate Condition
[Entity Condition Types](../entity_condition_types.md)

Evaluates an entity condition that is stored in a file.

Type ID: `ra_additions:evaluate_condition`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `entity_condition` | [String](../data_types/string.md) | _optional_ | The Identifier of the tag or condition file to be evaluated | 

### Example
```json
{
  "type": "ra_additions:evaluate_condition",
  "entity_condition": "test_pack:active_power_type_example"
}
```
This example will check the `test_pack:active_power_type_example` entity condition.
