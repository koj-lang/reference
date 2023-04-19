# Type Declarations

> **<sup>Syntax</sup>**\
> _TypeDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` `type` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) `=`
>  [_Type_](/type_system/index.md) `;`

Type declarations can be used both to alias existing types or create new ones. The identifiers on the right-hand side of an equal sign, the right-hand side of the colon in struc fields and in enums must correspond to existing already types.

Example:

You can define a `Pizza` type representing a recipe for a pizza in the following way:

```
let type Pizza = struct {
  .crust: enum `Thick | `Thin | `Cheesy;
  .base: enum `Tomato | `Cream;
  .toppings: [string];
}
```
