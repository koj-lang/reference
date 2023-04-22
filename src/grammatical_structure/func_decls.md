# Function Declarations

> **<sup>Syntax</sup>**\
> _FuncDecl_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `let` `func` [IDENTIFIER](/lexical_structure/identifiers.md) `=`\
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `(` _FuncDeclArgs_<sup>?</sup> `)` `=>` _Expression_
>
> _FuncDeclArgs_ :\
> _FuncDeclArg_ ( `,` _FuncDeclArg_ )<sup>*</sup>
>
> _FuncDeclArg_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [IDENTIFIER](/lexical_structure/identifiers.md) `:` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) 
