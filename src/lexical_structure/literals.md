# Literals

Literals are used to represent values in the source code. They are used to initialize variables, to pass arguments to functions, etc.

## Integer literals

Integer literals represent an integer value. They can be written in decimal, hexadecimal, octal or binary notation.

> INTEGER_LITERAL := DECIMAL_LITERAL | HEXADECIMAL_LITERAL | OCTAL_LITERAL | BINARY_LITERAL
>
> DECIMAL_LITERAL := DEC_DIGIT*
>
> HEXADECIMAL_LITERAL := ( `0x` | `0X` )DEC_DIGIT+
>
> OCTAL_LITERAL := ( `0o` | `0O` )OCT_DIGIT+
>
> BINARY_LITERAL := ( `0b` | `0B` )BIN_DIGIT+
>
> BIN_DIGIT := [ `0` - `1` ]
>
> OCT_DIGIT := [ `0` - `7` ]
>
> HEX_DIGIT := [ `0` - `9` `a` - `f` `A` - `F` ]
>
> DEC_DIGIT := [ `0` - `9` ]

## Floating-point literals

Floating-point literals represent a floating-point value. They can be written in decimal or hexadecimal notation.

> FLOATING_LITERAL :=
> | DECIMAL_LITERAL `.` DECIMAL_LITERAL?
> | `.` DECIMAL_LITERAL
> | DECIMAL_LITERAL ( `.` DECIMAL_LITERAL )? EXPONENT
>
> EXPONENT := ( `e`|`E` ) ( `+`|`-` )? DECIMAL_LITERAL

## String and character literals

Character literals represent a single character. String literals represent a sequence of characters.

### Character literals

> CHAR_LITERAL : `'` ( ~[ `'` `\` `\n` `\r` `\t` ] | QUOTE_ESCAPE | ASCII_ESCAPE | UNICODE_ESCAPE ) `'`
>
> QUOTE_ESCAPE : `\'` `\"`
>
> ASCII_ESCAPE : `\x` OCT_DIGIT HEX_DIGIT | `\n` | `\r` | `\t` | `\\` | `\0`
>
> UNICODE_ESCAPE : `\u{` HEX_DIGIT[1,6] `}`

### String literals

> STRING_LITERAL : `"` ( ~[ `"` `\` `\n` `\r` `\t` ] | QUOTE_ESCAPE | ASCII_ESCAPE | UNICODE_ESCAPE )* `"`
