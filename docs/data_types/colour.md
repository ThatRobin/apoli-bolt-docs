# Colour Holder

[Data Type](../data_types.md).

An [Object](object.md) that holds RGBA values

!!! note
		The name of this Data Type is "colour", not "color"! Be careful not to misspell it!

### Fields:

Field  |      Type         | Default | Description
-------|-------------------|---------|-------------
`red`  | [Float](float.md) | 1.0 | Value by which the red component of the texture will be multiplied. Range: 0 - 1
`green`| [Float](float.md) | 1.0 | Value by which the green component of the texture will be multiplied. Range: 0 - 1
`blue` | [Float](float.md) | 1.0 | Value by which the blue component of the texture will be multiplied. Range: 0 - 1
`alpha`| [Float](float.md) | 1.0 | Value by which the alpha (= transparency) component of the texture will be multiplied. Range: 0 - 1

### Examples:

```json
"colour": {
	"red": 1,
	"green": 0,
	"blue": 0
}
```

This definition results in a red colour.
<br>

```json
"colour": {
	"red": 0,
	"green": 0,
	"blue": 1,
	"alpha": 0.5
}
```
This definition results in a blue colour with half opacity.
