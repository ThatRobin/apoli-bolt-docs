# Attributed Attribute Modifier
[Data Type](../data_types.md)

An [Object](object.md) used to specify how a specific attribute should be modified. Basically an [Attribute Modifier](attribute_modifier.md) with an additional `attribute` field.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `attribute` | [Identifier](identifier.md) |   | ID of the attribute which will be modified by this modifier. | 
 | `operation` | [Attributed Attribute Modifier Operation](attributed_attribute_modifier_operation.md) |   | The operation which will be performed by this modifier. | 
 | `value` | [Float](float.md) |   | The value to use for the modifier operation. | 
 | `name` | [String](string.md) | _optional_ | A descriptive name for the modifier, describing where it comes from. | 

