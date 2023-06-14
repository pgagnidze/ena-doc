---
title: ენის სინტაქსი
description: ენას სინტაქსის ინსტრუქცია.
---

დასაშვებია ინგლისური სიტყვებისა და ასოების გამოყენებაც სწავლის პროცესის გასამარტივებლად.

## Booleans

Booleans are either ჭეშმარიტი or მცდარი.

Example:

```lua
ფუნქცია მთავარი() {
  მაჩვენე ჭეშმარიტი
  მაჩვენე მცდარი
}
```

Output:

```lua
true
false
```

## Numerals

Numerals support bases (e.g., decimal, binary, octal, or hexadecimal) and exponential notation.

Example:

```lua
ფუნქცია მთავარი() {
  მაჩვენე 01 1010 # binary
  მაჩვენე 07 12 # octal
  მაჩვენე 0f A # hexadecimal
  მაჩვენე 1e3 # exponential notation
}
```

Output:

```lua
10
10
10
1000
```

## Strings

Strings are enclosed in either double quotes or single quotes. special characters are escaped automatically. Strings can be concatenated using the + operator.

Example:

```lua
ფუნქცია მთავარი() {
  ა = "გამარჯობა"
  მაჩვენე ა + " სამყარო"
}
```

Output:

```lua
გამარჯობა სამყარო
```

## Function declaration

Functions are declared using the ფუნქცია keyword, followed by the function name, a list of parameters enclosed in parentheses, and a block of code.

Example:

```lua
ფუნქცია მთავარი() {
  დააბრუნე ჭეშმარიტი
}
```

Result:

```lua
true
```

## Function call

Functions are called using the function name, followed by a list of arguments enclosed in parentheses.

Example:

```lua
ფუნქცია ფაქტორიალი(ნ = 6) {
  თუ ნ != 0 {
      დააბრუნე ნ * ფაქტორიალი(ნ - 1)
  } თუარა {
      დააბრუნე 1
  }
}
ფუნქცია მთავარი() {
    დააბრუნე ფაქტორიალი()
}
```

Result:

```lua
720
```

## Variables

variables are assigned using variable name, an equals sign, and the new value.

Example:

```lua
ფუნქცია მთავარი() {
  ა = 1
  მაჩვენე ა
}
```

Output:

```lua
1
```

## Return

the return keyword is used to return a value from a function. It can also have an expression.

Example:

```lua
ფუნქცია მთავარი() {
  დააბრუნე 1 + 1
}
```

Result:

```lua
2
```

## Arrays

when creating an array you use ახალი keyword. Followed by open and close brackets; inside the brackets you can put any value you want to indicate the size. Finally it has default value. Array indexing starts from 1** not 0 like in most programming languages.

Example:

```lua
ფუნქცია მთავარი() {
  მასივი = ახალი[5] 0
  მასივი[1] = 1
  მაჩვენე მასივი
}
```

Output:

```lua
[1, 0, 0, 0, 0]
```

We can create multidimensional arrays by nesting arrays.
Example:

```lua
ფუნქცია მთავარი() {
  მასივი = ახალი[2][2] 0
  მასივი[1][1] = 1
  მასივი[1][2] = 2
  მასივი[2][1] = 3
  მაჩვენე მასივი
}
```

Output:

```lua
[
 [1, 2],
 [3, 0]
]
```

## If statements

თუ, თუარა, and თუარადა are used for conditional execution. Expressions doesn't need to be surrounded by parentheses. The body of each branch must be surrounded by curly braces.

Example:

```lua
ფუნქცია მთავარი() {
  ციფრი = 5
  თუ ციფრი > 0 {
    მაჩვენე ციფრი
  } თუარადა ციფრი < 0 {
    მაჩვენე "ციფრი ნაკლებია ნულზე"
  } თუარა {
    მაჩვენე "ციფრი არის ნული"
  }
}
```

Output:

```lua
5
```

## While statements

სანამ is used for while looping.

Example:

```lua
ფუნქცია მთავარი() {
  ციფრი = 5
  სანამ ციფრი > 0 {
    მაჩვენე ციფრი
    ციფრი = ციფრი - 1
  }
}
```

Output:

```lua
5
4
3
2
1
```

## Shell Commands

ბრძანება or $ is used for executing shell commands.

Example:

```lua
ფუნქცია მთავარი() {
  ბრძანება "echo გამარჯობა, მსოფლიო!"
}
```

Output:

```lua
გამარჯობა, მსოფლიო!
```

or

```lua
ფუნქცია მთავარი() {
  $ "echo გამარჯობა, მსოფლიო!"
}
```

Output:

```lua
გამარჯობა, მსოფლიო!
```

## Print

მაჩვენე or @ is used for printing.

Example:

```lua
ფუნქცია მთავარი() {
  მაჩვენე "გამარჯობა, მსოფლიო!"
}
```

Output:

```lua
გამარჯობა, მსოფლიო!
```

or

```lua
ფუნქცია მთავარი() {
  @ "გამარჯობა, მსოფლიო!"
}
```

Output:

```lua
გამარჯობა, მსოფლიო!
```

## Comments

single-line comments start with # and continue until the end of the line. Multi-line comments start with #{ and end with #}.

Example:

```lua
ფუნქცია მთავარი() {
  მაჩვენე "გამარჯობა, მსოფლიო!" # This is a comment.
  #{
    This is a multi-line comment.
    This is a comment.
  #}
}
```
