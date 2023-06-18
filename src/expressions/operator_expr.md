# Operator Expressions

> **<sup>Syntax</sup>**\
> _OperatorExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [_ArithmeticOpExpression_](#arithmetic-operations)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_BitwiseOpExpression_](#bitwise-operations)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_LogicalOpExpression_](#logical-operations)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_ComparisonExpression_](#comparisons)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_AssignementExpression_](#assignements)\
> &nbsp;&nbsp;&nbsp;&nbsp; | _StringOpExpression_

## Arithmetic Operations

> **<sup>Syntax</sup>**\
> _ArithmeticOpExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `-` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `+` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `-` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `*` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `/` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `//` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `%` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `**` [_Expression_](/expressions/index.md)

These operators are, in order, the negation, addition, substraction, multiplication, division, integer division, modulo and exponentiation operators.

## Bitwise Operations

> **<sup>Syntax</sup>**\
> _BitwiseOpExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `~` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `&` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `|` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `^` [_Expression_](/expressions/index.md)

These operators represent, in order, the bitwise NOT, AND, OR and XOR operators.

## Logical Operations

> **<sup>Syntax</sup>**\
> _LogicalOpExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `!` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `&&` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `||` [_Expression_](/expressions/index.md)

These operator represent, respectively, the logical NOT, AND and OR operators.

## Comparisons

> **<sup>Syntax</sup>**\
> _ComparisonExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [_Expression_](/expressions/index.md) `>` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `>=` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `<` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `<=` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `==` [_Expression_](/expressions/index.md)\
> &nbsp;&nbsp;&nbsp;&nbsp; | [_Expression_](/expressions/index.md) `!=` [_Expression_](/expressions/index.md)

These operators represent, in order, the greater than, greater or equal, less than, less than or equal, equal and not equal operators.

## Assignements

> **<sup>Syntax</sup>**\
> _AssignementExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [_Expression_](/expressions/index.md) `:=` [_Expression_](/expressions/index.md)

The expression on the left side of the operator must be assignable to (a *lvalue*). It must also not have been declared as `const`.

## String Operations

> **<sup>Syntax</sup>**\
> _StringOpExpression_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; [_Expression_](/expressions/index.md) `@` [_Expression_](/expressions/index.md)

This operator represents the string concatenation.
