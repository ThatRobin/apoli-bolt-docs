# Key
[Data Type](../data_types.md)

An [Object](object.md) which defines a keybinding, used in active powers to define which key they react to.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `key` | [String](string.md) |   | A string specifying the keybinding. See [Keybindings](../../misc/extras/keybindings.md) for possible values. | 
 | `continuous` | [Boolean](boolean.md) | `false` | Whether the keybinding should only trigger the power on the first tick the key is held down, or, if set to true, continuously on each tick while the key is held. | 

