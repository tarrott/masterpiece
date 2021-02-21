---
title: "Golang"
date: 2021-01-31T08:43:58-05:00
draft: false
weight: 3
---


## Packages
- programs start running in `package main`
- package name is the same as the as the last element of the import path (`"math/rand"`) is comprised of files wtih `package rand`
- only names beginning with Capital letters are exported (and available) outside of packages

## Variables
- `var` delcares a list of variables of the same type (`var i, j, k int`)
    - multiple `var` declarations can be grouped similar to package imports
- if the `var` is initialized then the type can be omitted (`var i, j = 1, 2`)
- short hand `:=` declaration can only be used within functions
- `%T` will print out a variables type

## Functions
- first-class functions
- naked returns (only use in short functions) return the named return values 
    - `func split(sum int) (x, y int) {... return}` will return `x` and `y`

## Data Types
- int/unit (platform dependent)
    - [int  int8  int16  int32  int64]
    - [uint uint8 uint16 uint32 uint64 uintptr]
- byte (alias for uint8)
- rune (alias for int32)
- float32
- float64 (default float type)
- string
- bool

## Pointers
- no pointer arithmetic, unlike C

## Control Flow
- `for` - no parentheses surround the expression, just the `{}`
    - while loops are written as simple `for` loops (`for i<10{fmt.Println("Hello")}`>)
- `switch` - stops execution once a valid case is hit
    - no expressions will default to `true` (`switch true(...)`)
- `defer` - called after the containing function completes
    - multiple `defer` statments gets called LIFO (last in, first out)

## Structs
- `type Vertex struct { X, Y float64 }`
- no classes but `type`/`struct` can have methods

## Arrays & Slices
- created by built-in `make` function
    - `make([]array_type, length int, capacity int)`
- slices do not store data, only reference underlying arrays
- changing a slice updates the referenced array and any other slice referencing that array
- appending a list returns a slice, allocating a bigger underlying array if required
    - `var s []int`
    - `s = append(s, 1, 2, 3)`
- `range` in a `for` loop returns two values for each iteration, index & value
    - `pow = []int{1, 2, 4, 8}`
    - `for i, v := range pow {...}`

## Maps
- initialize with `make` function
    - `m = make(map[string]string)`
- delete an element from a map with `delete(m, key)`
- check if key exists with two-value assignment `elem, ok := m[key]`


## Routines
