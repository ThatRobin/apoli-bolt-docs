---
title: Damage (Bi-entity Action Type)
date: 2024-08-25
---

# Damage

[Bi-entity Action Type](../bientity_action_types.md)

Add the target entity to the power that uses the [Entity Set (Power Type)](../power_types/entity_set.md) of the actor entity.

Method Name: `.damage()`


### Arguments

| Field          | Type                                    | Optional   | Description                                                                                                  |
|----------------|-----------------------------------------|------------|--------------------------------------------------------------------------------------------------------------|
| `amount`       | [Float](../data_types/float.md)         |            | The amount of damage to deal.                                                             | 
| `damage_type`  | [String](../data_types/string.md)       |            | Defines the properties of the damage source that will be dealt, such as part of its death message, and whether it can bypass armor, shield, etc. (via damage type tags.) | 
| `modifier`     | [Object](../data_types/object.md)       | *optional* | If specified, this modifier will be applied to the damage taken by the 'target' entity.   | 
| `modifiers`    | [Object](../data_types/object.md)       | *optional* | If specified, these modifiers will be applied to the damage taken by the 'target' entity. | 


!!! Note
    There is no example usage of this type yet.

=== "Apoli-Bolt"
    ```py

    ```
=== "Json"
    ```json
    
    ```