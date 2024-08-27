---
title: Add Block (Block Action Type)
date: 2024-08-25
---

# Add Block

[Block Action Type](../block_action_types.md)

Adds a block at the specified action position. Adding means setting the block at the position, offset by the direction of the action.

Method Name: `.explode()`


### Arguments

| Field   | Type                                      | Default | Description                                 |
|---------|-------------------------------------------|----------|---------------------------------------------|
| `power` | [Float](../data_types/float.md) |          | Determines the power of the explosion. | 
| `destruction_type` | [Destruction Type](../data_types/destruction_type.md) | `"break"` | Determines the effect of the explosion to the terrain. | 
| `indestructible` | [Block Condition Type](../block_condition_types.md) | *optional* | If specified, the blocks that fulfill this condition will not be destroyed by the summoned explosion. | 
| `destructible` | [Block Condition Type](../block_condition_types.md) | *optional* | If specified, only the blocks that fulfill this condition will be destroyed by the summoned explosion. | 
| `create_fire` | [Boolean](../data_types/boolean.md) | `false` | Determines if the summoned explosion should create fire. | 


!!! Note
    There is no example usage of this type yet.

=== "Apoli-Bolt"
    ```py

    ```
=== "Json"
    ```json
    
    ```