# Status Effect Instance
[Data Type](../data_types.md)

An [Object](object.md) used to define a status effect with duration, amplifier, etc.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `effect` | [Identifier](identifier.md) |   | ID of the status effect. | 
 | `duration` | [Integer](integer.md) | `100` | Duration of the status effect in ticks. | 
 | `amplifier` | [Integer](integer.md) | `0` | Amplifier of the status effect. | 
 | `is_ambient` | [Boolean](boolean.md) | `false` | Whether the effect counts as an ambient effect. | 
 | `show_particles` | [Boolean](boolean.md) | `true` | Whether the status effect will spawn particles on the player. | 
 | `show_icon` | [Boolean](boolean.md) | `true` | Whether the status effect will show an icon on the HUD. | 

