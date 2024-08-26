---
title: Add To Set (Bi-entity Action Type)
date: 2024-08-25
---

# Add To Set

[Bi-entity Action Type](../bientity_action_types.md)

Add the target entity to the power that uses the [Entity Set (Power Type)](../power_types/entity_set.md) of the actor entity.

Method Name: `.add_to_set()`


### Arguments

| Field         | Type                                    | Default   | Description                                                                                                  |
|---------------|-----------------------------------------|------------|--------------------------------------------------------------------------------------------------------------|
| `set`         | [String](../data_types/string.md)       |            | The ID of the power to add the target entity into.                                                           | 
| `time_limit`  | [Integer](../data_types/power_phase.md) | *optional* | If specified, this will determine how long the target entity will be stored in the specified power in ticks. | 


!!! Note
    There is no example usage of this type yet.

=== "Apoli-Bolt"
    ```py

    ```
=== "Json"
    ```json
    
    ```