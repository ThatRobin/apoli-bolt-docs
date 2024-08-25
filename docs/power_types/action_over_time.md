---
title: Action Over Time (Power Type)
date: 2024-08-24
---

# Action Over Time

[Power Type](../power_types.md)

Type ID: `apoli:action_over_time`


### Methods

| Field       | Type | Description | 
|-------------|------|-------------|
| `get_phase` | [PowerPhase](../data_types/power_phase.md) | Determines the phase of the Action Over Time to use. | 


??? Note
    You cannot use PowerPhases with `if-else` statements, due to the nature of how apoli parses json, the `else` is unabable to be parsed, and will result in a warning in the console.

=== "Apoli-Bolt"
    ```py
    @power(
        type="apoli:action_over_time", 
        condition=entity.is_on_fire(),
        interval=20
    )
    def phase_example(power: ActionOverTimePower):
        if power.get_phase() == PowerPhase.RISING:
            say "condition is now fulfilled"
        if power.get_phase() == PowerPhase.FALLING:
            say "condition is no longer fulfilled"
        
        # This will happen constantly:
        say "condition is constantly fulfilled"

        # This is another way to write a constant action:
        if power.get_phase() == PowerPhase.CONSTANT:
            say "condition is constantly fulfilled again"
    ```
=== "Json"
    ```json
    {
        "type": "apoli:action_over_time",
        "rising_action": {
            "type": "apoli:execute_command",
            "command": "say \"condition is now fulfilled\""
        },
        "falling_action": {
            "type": "apoli:execute_command",
            "command": "say \"condition is no longer fulfilled\""
        },
        "entity_action": {
            "type": "apoli:and",
            "actions": [
                {
                    "type": "apoli:execute_command",
                    "command": "say \"condition is constantly fulfilled\""
                },
                {
                    "type": "apoli:execute_command",
                    "command": "say \"condition is constantly fulfilled again\""
                }
            ]
        },
        "interval": 20,
        "condition": {
            "type": "apoli:on_fire"
        }
    }
    ```