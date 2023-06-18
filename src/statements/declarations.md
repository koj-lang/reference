# Declarations

> **<sup>Syntax</sup>**\
> _Declaration_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; _VarDecl_ | _FuncDecl_

## Variable Declarations

> **<sup>Syntax</sup>**\
> _VarDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` _Mutability_ [IDENTIFIER](/lexical_structure/identifiers.md) ( `:` [_Type_](/type_system/index.md) )<sup>?</sup> `:=` _Expression_
>
> _Mutability_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `mut` | `const`

Variables can be declared as either `mut` or `const`. `const` variables can not be assigned a value after they are declared.

## Function Declarations

> **<sup>Syntax</sup>**\
> _FuncDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` `func` [IDENTIFIER](/lexical_structure/identifiers.md) `:=`\
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `(` _FuncDeclArgs_<sup>?</sup> `)` `=>` _Expression_
>
> _FuncDeclArgs_ :\
> _FuncDeclArg_ ( `,` _FuncDeclArg_ )<sup>\*</sup>
>
> _FuncDeclArg_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [IDENTIFIER](/lexical_structure/identifiers.md) `:` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md)
