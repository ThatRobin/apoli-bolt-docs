# Boss Bar Hud Render Overlay
[Data Type](../data_types.md)

An [Object](object.md) used to define how a boss bar overlay should be rendered.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | should_render | [Boolean](../data_types/boolean.md) | _optional_ | Whether the bar should be visible or not. | 
 | bar_index | [Int](../data_types/int.md) | _optional_ | The indexed position of the bar on the sprite to use. Please note that indexes start at 0. | 
 | priority | [Int](../data_types/int.md) | _optional_ | The order in which the bar appears on the screen. | 
 | sprite_location | [Identifier](../data_types/identifier.md) | _optional_ | The path to the file in the assets which contains what the bar looks like. | 

### Example
```json
{
  "sprite_location": "textures/gui/bars.png",
  "bar_index": 1,
  "should_render": true,
  "condition": {
    "type": "apoli:exposed_to_sun"
  }
}
```

