---
title: ენის წესები
description: ენის გამოყენების წესები და შესღუდვები.
---

ამ დოკუმენტში გაგაცნობთ ენის შეზღუდვებსა და გამოყენების წესებს.

## Array indexing

Array indexing starts from 1 not 0 like in most programming languages.

## Statement

Statemenet separator ";" is optional. Statements are separated by newlines.

## Identifier

identifiers are allowed to contain the letters ა-ჰ, the digits 0-9, and underscores. Identifiers must start with a letter or an underscore. Identifiers are case-sensitive.
For Example: ცვლადი, ცვლადი_2, ცვლადი2,_ცვლადი, _ცვლადი2

## Numeral base notation

Digits 0-9 are used in numerals. Indicate non-decimal bases using "0val", with val ranging from 0-9 and a-z.
Examples:

- "123" - Decimal for 123.
- "00 1" - Binary for 1.
- "01 10" - Base 2 for 2.
- "02 11" - Base 3 for 4.
- "0e 13" - Base 15 for 18.
- "0f 14" - Base 16 for 20.
Octal, Hexadecimal, and Binary can be represented as:
- "07 21" - Octal for 7.
- "0f 210" - Hexadecimal for 15.
- "01 10" - Binary for 2.
Or in a format with "b":
- "10 b2" - Binary for 2.
- "170 b8" - Octal for 120.
- "FF00 b16" - Hexadecimal for 65280.

## Numeral exponent notation

Exponential notation represents scientific numbers. It includes a base, "e" (lowercase or uppercase), and an exponent.
Examples:
"1e2" or "1E2" - Equals 1 *10^2.
"1e-2" - Equals 1* 10^-2.

## Operators

Ena includes these operators:

- Arithmetic: +, -, *, /, %, ^
- Comparison: <, <=, >, >=, ==, !=
- Logical: &&, ||, !

Operator precedence from low to high:

- Logical: &&, ||
- Comparison: <, <=, >, >=, ==, !=
- Not: !
- Addition, subtraction: +, -
- Multiplication, division, modulo: *, /, %
- Unary minus: -
- Exponentiation: ^

## Falsy values

Falsy values are მცდარი, 0, and nil. All other values are truthy.

## Assignemnts

Addition assignemnts, subtraction assignemnts, multiplication assignemnts, division assignemnts, and modulus assignemnts are not allowed. Use the following instead: ა = ა + 1, ა = ა - 1, ა = ა * 1, ა = ა / 1, ა = ა % 1.

## Increment and decrement

Increment and decrement operators are not allowed. Use the following instead: ა = ა + 1, ა = ა - 1.

## Structured programming

Structured programming is enforced. This means that all code must be written inside functions. It has entrypoint function მთავარი which is called when the program starts. Entrypoint function doesn't take any parameters.
Example:

```lua
ფუნქცია მთელი_რიცხვი() {
    დააბრუნე ჭეშმარიტი
}
ფუნქცია მთავარი() {
    მთელი_რიცხვი()
}
```
