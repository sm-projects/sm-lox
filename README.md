# sm-lox

Implementing an interpreter for Lox language. Mainly taken from Bob Nystrom wonderful online book called [Crafting Compilers](http://craftinginterpreters.com/).
I started off, following the code and design used in the book and then deviated from it in order to incorporate my own design choices and also to learn and use tools such as Yacc and [Atllr](http://www.antlr.org/)

## Table of Contents
- [Introduction](#introduction)
- [The Lox Language](#theloxlanguage)
- [Features](#features)
- [Example](#example)
- [Optimizations](#optimizations)
- [FAQ](#faq)
- [API](#api)
- [Installation](#installation)
- [See Also](#see-also)
- [Support](#support)

---

## Introduction

## The Lox Language
```
expression → literal
           | unary
           | binary
           | grouping ;

literal    → NUMBER | STRING | "true" | "false" | "nil" ;
grouping   → "(" expression ")" ;
unary      → ( "-" | "!" ) expression ;
binary     → expression operator expression ;
operator   → "==" | "!=" | "<" | "<=" | ">" | ">="
           | "+"  | "-"  | "*" | "/" ;
```
## Resources
1. [AntLr Mega Tutorial](https://tomassetti.me/antlr-mega-tutorial/)
