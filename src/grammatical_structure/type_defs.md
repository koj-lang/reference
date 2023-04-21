# Type Declarations

> **<sup>Syntax</sup>**\
> _TypeDef_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `type` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) `=`
>  [_Type_](/type_system/index.md) `;`

Type declarations can be used both to alias existing types or create new ones.

Example:

You can define a `Pizza` type representing a recipe for a pizza in the following way:

```
type Pizza = struct {
  .crust: enum `Thick | `Thin | `Cheesy,
  .base: enum `Tomato | `Cream,
  .toppings: [String],
};
```
