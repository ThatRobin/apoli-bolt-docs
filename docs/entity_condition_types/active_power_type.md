# Active Power Type
[Entity Condition Types](../entity_condition_types.md)

Checks whether the entity has a power that uses the specified Power Type, excluding those in the blacklist, and is "active", meaning that the entity has the power and the power has all its conditions fulfilled.

Type ID: `ra_additions:active_power_type`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `power_type` | [Identifier](../data_types/identifier.md) | _optional_ | The namespace ID of the power type which will be checked to see if any are active. | 
 | `blacklisted_powers` | null | _optional_ | The namespace IDs of powers that will be excluded from the check. | 

### Example
```json
{
  "type": "ra_additions:active_power_type",
  "power_type": "apoli:elytra_flight",
  "blacklisted_powers": [
    "origins:elytra"
  ]
}
```
This example will check if the player has an elytra flight power that is not the elytrian's power.
