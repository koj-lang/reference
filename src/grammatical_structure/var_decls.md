# Variable Declarations

> **<sup>Syntax</sup>**\
> _VarDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` _Mutability_ [IDENTIFIER](/lexical_structure/identifiers.md) ( `:` [_Type_](/type_system/index.md) )<sup>?</sup> `=` _Expression_
>
> _Mutability_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `mut` | `const`

Variables can be declared as either `mut` or `const`. `const` variables can not be assigned a value after they are declared.
