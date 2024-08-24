# Boss Bar Hud Render
[Data Type](../data_types.md)

An [Object](object.md) used to define how a boss bar should be rendered.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | should_render | [Boolean](../data_types/boolean.md) | _optional_ | Whether the bar should be visible or not. | 
 | bar_index | [Int](../data_types/int.md) | _optional_ | The indexed position of the bar on the sprite to use. Please note that indexes start at 0. | 
 | priority | [Int](../data_types/int.md) | _optional_ | The order in which the bar appears on the screen. | 
 | overlays | [Array](../data_types/array.md) of [Boss Bar Hud Render Overlays](../data_types/boss_bar_hud_render_overlay.md) | _optional_ | The overlays you can display on the boss bar. | 
 | sprite_location | [Identifier](../data_types/identifier.md) | _optional_ | The path to the file in the assets which contains what the bar looks like. | 

### Example
```json
{
  "should_render": true,
  "bar_index": 0,
  "side": "right",
  "sprite_location": "example_pack:textures/gui/icons.png"
}
```

