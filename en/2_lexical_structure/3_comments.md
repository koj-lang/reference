---
title: 'Comments'
index: 3
---

## Comments

Comments are used to document the code and are ignored by the compiler.

There are two types of comments:

- Single-line comments start with `//` and end at the end of the line.
- Block comments start with `/*` and end with `*/`. They can span multiple lines.

> COMMENT := LINE_COMMENT | BLOCK_COMMENT
>
> LINE_COMMENT := `//`[^`\n`]*
>
> BLOCK_COMMENT := `/``*`.*?`*``/`
