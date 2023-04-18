# Type Declarations

> **<sup>Syntax</sup>**\
> _TypeDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` `type` [IDENTIFIER](/lexical_structure/identifiers.md) `=`\
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [IDENTIFIER](/lexical_structure/identifiers.md) | _Struct_ | _Enum_\
> &nbsp;&nbsp;&nbsp;&nbsp; `;`
>
> _Struct_ :\
> &nbsp;&nbsp;&nbsp;&nbsp;`{`\
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_FieldDec_<sup>+</sup> `;`\
> &nbsp;&nbsp;&nbsp;&nbsp;`}`
>
> _FieldDec_:\
> &nbsp;&nbsp;&nbsp;&nbsp;`.` [IDENTIFIER](/lexical_structure/identifiers.md) `:` [IDENTIFIER](/lexical_structure/identifiers.md)
>
> _Enum_:\
> &nbsp;&nbsp;&nbsp;&nbsp; [IDENTIFIER](/lexical_structure/identifiers.md) ( `|` [IDENTIFIER](/lexical_structure/identifiers.md))<sup>*</sup>

Type declarations can be used both to alias existing types or create new ones. The identifiers on the right-hand side of an equal sign, the right-hand side of the colon in struc fields and in enums must correspond to existing already types.

Example:

You can define a `Point` type representing a point in 2D space in the following way:

```
let type Point = {
  .x: int;
  .y: int;
}
```
