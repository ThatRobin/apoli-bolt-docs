# Evaluate Condition
[Bientity Condition Types](../bientity_condition_types.md)

Evaluates a bi-entity condition that is stored in a file.

Type ID: `ra_additions:evaluate_condition`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `bientity_condition` | [String](../data_types/string.md) | _optional_ | The Identifier of the tag or condition file to be evaluated | 

### Example
```json
{
  "type": "ra_additions:evaluate_condition",
  "bientity_condition": "test_pack:test_condition"
}
```
This example will check the `test_pack:test_condition` item condition.
