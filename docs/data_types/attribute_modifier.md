# Attribute Modifier
[Data Type](../data_types.md)

An [Object](object.md) used to specify how a value should be modified.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `operation` | [Attribute Modifier Operation](attribute_modifier_operation.md) |   | The operation which will be performed by this modifier. | 
 | `value` | [Float](float.md) |   | The value to use for the modifier operation. | 
 | `resource` | [Identifier](../data_types/identifier.md) | _optional_ | If specified, the value of this power will be used instead of the value specified in the `value` field. | 
 | `name` | [String](string.md) | _optional_ | A descriptive name for the modifier, describing where it comes from. | 
 | `modifier` | [Attribute Modifier](attribute_modifier.md) | _optional_ | If specified, this modifier will be applied to the value of the modifier. | 

