# Introduction

> **Disclaimer** : this specification is going to change a lot as the language evolves. It is still a very new project and nothing is set in stone yet.

The `koj` language was born as a side project of mine after taking a class on compilers for my second year at TELECOM Nancy.

## Syntax

The goal for the syntax of this language is for it to be as _consistent_ as possible. Each syntactic construct should have one function and one function only.

## Implementation

The first iteration of this language is going to be implemented using an interpreter written in Ocaml, using [sedlex](https://github.com/ocaml-community/sedlex) as a lexer and [menhir](http://gallium.inria.fr/~fpottier/menhir/) as a parser. This language may then evolve to be a compiled one, probably implemented in itself with a hand-written lexer and parser and leveraging [LLVM](https://llvm.org/) as a backend.
