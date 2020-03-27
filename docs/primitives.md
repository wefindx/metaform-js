# Primitives

Primitives are the building blocks of complex data and everything metaform. It is recommended that you use these primitives instead of encapsulated primitives for performance and compatibility.

## Primitive types

* `null`: if a field is typed `null`, the value should also be `null`, which represents non-existing data or noops.
* `boolean`: if a field is typed `boolean`, it can be either `true` or `false`, which represents a boolean variable.
* `number`: if a field is typed `number`, it can be integers, fractions, zero, irrationals, or complex (`x + yi`). For example: `pi, 3, 7/9, 9+2i`. For more information, see the implementation notes below.
* `string`: a string encoded in unicode. For example: `"Hello world!", "你好世界！", "👌"`.

## Constructive primitive types

These primitive types describe ways to combine or transform other primitive types into something new.

* `array`: an ordered list of elements. Elements can be of any type.
* `ulist`: an unordered list of elementso of any type.
* `keyvalue`: a pair of two elements: first one is a `string` representing the key, the second one is an element of any type representing the value.
* `object`: an unordered list (`ulist`) of `keyvalue` elements.
* `ref`: a reference to a metaform-compatible resource. See also: [metaform-uri](metaform-uri.md). We will try to be as lazy as possible and leverage parallel computing for performance optimization and compatibility purposes.
* `lambda-abs`, `lambda-app`: you can implement lambda calculus directly in metaform! Because lambda calculus is turing complete, you can implement your favorite algorithms using lambda calculus and our presets. See also: [lambda-calculus](lambda-calculus.md). We will try to be as lazy as possible and leverage parallel computing for performance optimization and compatibility purposes.
