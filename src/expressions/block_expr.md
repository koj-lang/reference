# Block Expressions

> **<sup>Syntax</sup>**\
> _BlockExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `{` _BlockComponents_<sup>?</sup> `}`
>
> _BlockComponents_ :\
> &nbsp;&nbsp;&nbsp;&nbsp;  [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Statements_](/statements/index.md)<sup>+</sup>\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Statements_](/statements/index.md)<sup>+</sup> [_Expression_](/expressions/index.md)<sup>?</sup>

Block expressions are a way to chain several statements together. The value of a block expression is that of the last executed instruction.
