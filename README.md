
# Documentation
Learn everything you need about BktLang.

Bkt is a typed and compiled functional programming language, similar to Javascript, it take from Rust, Go and Elixir.

The goal of Bkt is to be very simple and easy to learn.

<br>

#### What's New
- First public release of the documentation that show how it'll work.


### `Installation`


### `Table of contents`
#### **Version 1.0-beta.1**

*The following documentation presentation is inspired by the V doc as starting point.* *

<table>
    <tr><td width=33% valign=top>

* [Entrypoint](#entrypoint)
* [Functions](#functions)
    * [Declaring functions](#declare-functions)
    * [Returning multiple values](#return-multiple-values)
* [Comments](#comments)
* [Running your code](#running-codes)
* [Variables](#variables)
* [Types](#types)
    * [Typing & casting](#typing-and-casting)
    * [Strings](#strings)
    * [Numbers](#numbers)
    * [Arrays](#arrays)
    * [Maps](#maps)
* [Declaring modules](#declare-modules)
* [Modules imports](#module-imports)
* [Symbol visibility](#symbol-visibility)
* [Statements & expressions](#statements--expressions)
    * [If](#if)
    * [Iterator (Map, Filter and Reduce)](#iterator)
    * [Match](#match)
    * [Pattern maching](#pattern-maching)
* [Structs](#structs)
    * [Optional and required field](#optional-and-required-field)
    * [Default field values](#default-field-values)
    * [Short struct literal syntax](#short-struct-literal-syntax)
    * [Access modifiers](#access-modifiers)
    * [Methods](#methods)

</td><td width=33% valign=top>

* [Functions 2](#functions-2)
    * [Pure functions by default](#pure-functions-by-default)
    * [Mutable arguments](#mutable-arguments)
    * [Anonymous & higher-order functions](#anonymous--higher-order-functions)
    * [Pipes](#pipes)
* [References](#references)
* [Constants](#constants)
* [Type Declarations](#type-declarations)
    * [Interfaces](#interfaces)
    * [Enums](#enums)
    * [Option/Result types & error handling](#optionresult-types-and-error-handling)
* [Generics](#generics)
* [Concurrency](#concurrency)
    * [Spawning Concurrent Tasks](#spawning-concurrent-tasks)
    * [Channels](#channels)
* [Decoding JSON](#decoding-json)
* [Testing](#testing)

</td><td valign=top>

* [Writing documentation](#writing-documentation)

</td></tr>
</table>

________
<br>

### `Entrypoint`

There is no real entrypoint in Bkt, the whole file is the entrypoint and any functions, types definition and contants is executed before code.

By respecting this rule, your can write the following code inside the file `index.bkt` of your project :

```
println(add(77, 33))

fn add(int x, int y) int {
	return x + y
}

fn sub(int x, int y) int {
	return x - y
}

println(sub(100, 50))
```

This code will print `110` followed by `50`.
