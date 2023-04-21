# Struct Types

> **<sup>Syntax</sup>**\
> _Struct_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `struct` `{` _StructFields_<sup>*</sup> `}`
>
> _StructFields_ : \
> &nbsp;&nbsp;&nbsp;&nbsp; _StructFieldDec_ ( `,` _StructFieldDec_ )<sup>*</sup> `,`<sup>?</sup>
> 
> _StructFieldDec_:\
> &nbsp;&nbsp;&nbsp;&nbsp;`.` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) `:` [_Type_](/type_system/index.md)

Structs are used to represent objects with fields. They are analogous to _structs_ in C or _record types_ in languages such as OCaml.

Example:

You may create a struct representing a point in 2D space the following way:

```
struct {
  .x: int,
  .y: int,
}
```
