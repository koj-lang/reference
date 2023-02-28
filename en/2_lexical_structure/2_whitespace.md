---
title: "Whitespace"
index: 2
---

## Whitespace

The `koj` language uses the following whitespace characters:

- `' '` (U+0020 SPACE)
- `'\t'` (U+0009 CHARACTER TABULATION)
- `'\n'` (U+000A LINE FEED)
- `'\r'` (U+000D CARRIAGE RETURN)
- U+000B LINE TABULATION
- U+000C FORM FEED
- U+0085 NEXT LINE
- U+200E LEFT-TO-RIGHT MARK
- U+200F RIGHT-TO-LEFT MARK
- U+2028 LINE SEPARATOR
- U+2029 PARAGRAPH SEPARATOR

These characters are called _whitespace characters_ and are used to separate tokens in the language. They are not part of the language and are ignored by the lexer.

The meaning of the program is preserved if any whitespace character is replaced by another one.
