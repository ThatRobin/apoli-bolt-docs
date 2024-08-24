# Attack
[Bientity Action Types](../bientity_action_types.md)

The actor entity will damage the target enemy as if they had just been hit with the weapon in the actors hand.

Type ID: `ra_additions:attack`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `source` | [Damage Source Description](../data_types/damage_source_description.md) | _optional_ |  | 
 | `damage_type` | [Damage Type](../data_types/damage_type.md) | _optional_ |  | 
 | `allow_enchants` | [Boolean](../data_types/boolean.md) | _optional_ | Should enchantments be taken into account in the attack. | 
 | `allow_weapons` | [Boolean](../data_types/boolean.md) | _optional_ | Should weapons/tools be taken into account in the attack. | 
 | `allow_effects` | [Boolean](../data_types/boolean.md) | _optional_ | Should effects be taken into account in the attack. | 
 | `allow_attributes` | [Boolean](../data_types/boolean.md) | _optional_ | Should attributes be taken into account in the attack. | 

### Example
```json
{
  "type": "ra_additions:attack",
  "allow_enchants": true,
  "allow_weapons": true,
  "allow_effects": true,
  "allow_attributes": true,
  "source": {
    "name": "player",
    "bypasses_armor": true
  }
}
```
This example will attack the target using the targets weapons, enchants, status effects and attributes, whilst ignoring the targets armour.
