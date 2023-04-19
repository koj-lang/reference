# Struct Types

> **<sup>Syntax</sup>**\
> _Struct_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `struct` `{`\
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _StructFieldDec_<sup>+</sup> \
> &nbsp;&nbsp;&nbsp;&nbsp; `}`
>
> _StructFieldDec_:\
> &nbsp;&nbsp;&nbsp;&nbsp;`.` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) `:` [_Type_](/type_system/index.md) `;`

Structs are used to represent objects with fields. They are analogous to _structs_ in C or _record types_ in languages such as OCaml.

Example:

You may create a struct representing a point in 2D space the following way:

```
struct {
  .x: int;
  .y: int;
}
```
