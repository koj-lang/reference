# Function Types

> **<sup>Syntax</sup>**\
> _FunctionType_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `(` _FunctionTypeArguments_<sup>?</sup> `)` `->` [_Type_](/type_system/index.md) 
>
> _FunctionTypeArguments_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [_Type_](/type_system/index.md) ( `,` [_Type_](/type_system/index.md) )<sup>*</sup>

Example:

A function adding two integers together may have the following type:

```
(int, int) -> int
```

