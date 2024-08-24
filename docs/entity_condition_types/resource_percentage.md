# Resource Percentage
[Entity Condition Types](../entity_condition_types.md)

Checks the percentage of a resource.

Type ID: `ra_additions:resource_percentage`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `resource` | [Power Type](../data_types/power_type.md) | _optional_ | The Identifier of the power type that defines the resource which exists on the player. | 
 | `comparison` | [Comparison](../data_types/comparison.md) | _optional_ | How the value of the power that will be evaluated should be compared to the specified value. | 
 | `percentage` | [Int](../data_types/int.md) | _optional_ | The percentage value to compare the value of the power that will be evaluated to. `(e.g 50%)` | 

### Example
```json
{
  "type": "ra_additions:resource_percentage",
  "resource": "test_pack:test_resource",
  "comparison": "\u003e\u003d",
  "percentage": 75
}
```
This example will check if the `test_pack:test_resource` is above 75% full.
