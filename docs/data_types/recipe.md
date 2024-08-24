# Crafting Recipe
[Data Type](../data_types.md)

An [Object](object.md) specifying a shapeless or shaped crafting recipe. For some more information, view [the page on recipes on the MC wiki](https://minecraft.gamepedia.com/Recipe).
### Fields (both types)

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `type` | [Identifier](identifier.md) |  | The type of recipe. Either `minecraft:crafting_shaped` or `minecraft:crafting_shapeless`. Other recipe types are not supported. | 
 | `id` | [Identifier](identifier.md) |  | An ID for this recipe. Has to be unique among all recipes, otherwise there will be a conflict. | 
 | `result` | [Object](object.md) with an `item` [ID](identifier.md) and `count` [Integer](integer.md) |  | The result of the crafting. **Note that vanilla does _not_ support NBT tags in the result.** | 

### Fields (shapeless)

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `ingredients` | [Array](array.md) of [Ingredient](ingredient.md) |  | The items that need to be put in the crafting grid for the recipe. | 

### Fields (shaped)

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `pattern` | [Array](array.md) of [Strings](string.md) |  | Specifies the pattern, with each element representing one row. Use a single character to describe one item. A space means that position is empty. | 
 | `key` | [Identifier](identifier.md) |  | Specifies which character in the pattern corresponds to which [Ingredient](ingredient.md). | 

