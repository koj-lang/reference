# Enum Types

> **<sup>Syntax</sup>**\
> _Enum_ :\
> &nbsp;&nbsp;&nbsp;&nbsp; `enum` 
>  `{` _EnumMember_ ( `,` _EnumMember_ )<sup>*</sup> `,`<sup>?</sup> `}`\
>
> _EnumMember_ :
> `` ` `` [TYPE_IDENTIFIER](/lexical_structure/identifiers.md) ( _EnumMemberOfType_ )<sup>?</sup>
>
> _EnumMemberOfType_ :
> `(` [_Type_](/type_system/index.md) `)` 

Examples:

To represent a direction on a D-pad, you could use the following enum:

```
enum { `Up, `Down, `Left, `Right }
```

To represent a user on a website, you could use the following enum:

```
enum {
 `Anon,
 `LoggedIn(struct { id: string, role: string }),
}
```
