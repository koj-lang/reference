# Literals

Literals are used to represent values in the source code. They are used to initialize variables, to pass arguments to functions, etc.

## Integer literals

Integer literals represent an integer value. They can be written in decimal, hexadecimal, octal or binary notation.

> INTEGER_LITERAL :\
> &nbsp;&nbsp;&nbsp;&nbsp; DECIMAL_LITERAL\
> &nbsp;&nbsp;&nbsp;&nbsp; | HEXADECIMAL_LITERAL\
> &nbsp;&nbsp;&nbsp;&nbsp; | OCTAL_LITERAL\
> &nbsp;&nbsp;&nbsp;&nbsp; | BINARY_LITERAL
>
> DECIMAL_LITERAL : DEC_DIGIT<sup>*</sup>
>
> HEXADECIMAL_LITERAL : ( `0x` | `0X` )DEC_DIGIT<sup>+</sup>
>
> OCTAL_LITERAL : ( `0o` | `0O` )OCT_DIGIT<sup>+</sup>
>
> BINARY_LITERAL : ( `0b` | `0B` )BIN_DIGIT<sup>+</sup>
>
> BIN_DIGIT : [ `0` - `1` ]
>
> OCT_DIGIT : [ `0` - `7` ]
>
> HEX_DIGIT : [ `0` - `9` `a` - `f` `A` - `F` ]
>
> DEC_DIGIT : [ `0` - `9` ]

## Floating-point literals

Floating-point literals represent a floating-point value. They can be written in decimal or hexadecimal notation.

> FLOATING_LITERAL :\
> &nbsp;&nbsp;&nbsp;&nbsp; | DECIMAL_LITERAL `.` DECIMAL_LITERAL<sup>?</sup>\
> &nbsp;&nbsp;&nbsp;&nbsp; | `.` DECIMAL_LITERAL\
> &nbsp;&nbsp;&nbsp;&nbsp; | DECIMAL_LITERAL ( `.` DECIMAL_LITERAL )<sup>?</sup> EXPONENT
>
> EXPONENT := ( `e`|`E` ) ( `+`|`-` )<sup>?</sup> DECIMAL_LITERAL

## String and character literals

Character literals represent a single character. String literals represent a sequence of characters.

### Character literals

> CHAR_LITERAL : `'` CHAR_FRAGMENT<sup>?</sup> `'`
>
> CHAR_FRAGMENT :  
> &nbsp;&nbsp;&nbsp;&nbsp; ~[ `'` `\` `\n` `\r` `\t` ]\
> &nbsp;&nbsp;&nbsp;&nbsp; | QUOTE_ESCAPE\
> &nbsp;&nbsp;&nbsp;&nbsp; | ASCII_ESCAPE\
> &nbsp;&nbsp;&nbsp;&nbsp; | UNICODE_ESCAPE 
>
> QUOTE_ESCAPE : `\'` `\"`
>
> ASCII_ESCAPE : `\x` OCT_DIGIT HEX_DIGIT | `\n` | `\r` | `\t` | `\\` | `\0`
>
> UNICODE_ESCAPE : `\u{` HEX_DIGIT<sup>[1,6]</sup> `}`

### String literals

> STRING_LITERAL : `"` STRING_FRAGMENT<sup>*</sup> `"`
>
> STRING_FRAGMENT :\
> &nbsp;&nbsp;&nbsp;&nbsp; ~[ `"` `\` `\n` `\r` `\t` ]\
> &nbsp;&nbsp;&nbsp;&nbsp; | QUOTE_ESCAPE\
> &nbsp;&nbsp;&nbsp;&nbsp; | ASCII_ESCAPE\
> &nbsp;&nbsp;&nbsp;&nbsp; | UNICODE_ESCAPE
