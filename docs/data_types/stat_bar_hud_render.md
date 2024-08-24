# Stat Bar Hud Render
[Data Type](../data_types.md)

An [Object](object.md) used to define how a stat bar should be rendered.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | should_render | [Boolean](../data_types/boolean.md) | _optional_ | Whether the bar should be visible or not. | 
 | bar_index | [Int](../data_types/int.md) | _optional_ | The indexed position of the bar on the sprite to use. Please note that indexes start at 0. | 
 | side | [String](../data_types/string.md) | right | Determines which side of the players HUD the bar appears on. Can be `"left"` or `"right"`. | 
 | sprite_location | [Identifier](../data_types/identifier.md) | _optional_ | The path to the file in the assets which contains what the bar looks like. The base mod doesn't include any bars, but you can create your own using Resource Packs. | 

### Example
```json
{
  "should_render": true,
  "bar_index": 0,
  "side": "right",
  "sprite_location": "example_pack:textures/gui/icons.png"
}
```

