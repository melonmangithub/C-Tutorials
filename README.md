# An Introduction to the C Programming Langauge

## Preface 
This project will hopefully help explain C.

Does not cover setup, use repl.it for simplicity.

Enjoy (:

## Some background knowledge

### Variables and Types

Variables in C work like any other programming language, they are quite simply a location in your computers memory that holds a value.

However, in C, variables must be given an explicit *type*. So whats a type?

A type is the form of value that a variable holds. C has only a few base types

- **int**: a whole number
- **float**: a floating point (decimal) value
- **char**: a character

A float only holds 7 digits behind the decimal. Generally this is fine, however, to ensure reliability, id recommand the **double** for decimal values. As the name implies, its twice as large as a float, and holds 15 digits behind the decimal. So why would you even want to use the less precise float in the first place? Its mostly historical, as the float takes up 4 bytes of memory, while the double (unsuprisingly) takes up 8, so the float was favored to conserve memory. Its 2022 now, computers have processors and memory in magnitudes faster and larger than in the 70s or 80s, so using a double has no cons concerning memory. 

Also, id like to point out that the **char** type is not actually a character, rather a number that encodes a character. However you dont really need to know this, as chars are asigned using single quotes with the character you desire inside (eg, 'a', 'b', 'c'). The ascii encoding that C uses can be refrenced [here](https://ascii-tables.com/).

**int** can also have modifiers, **long**, **short**, **unsigned**, and **signed**. These go before the keyword **int** when you actually declare the variable.

As for the **long** and **short**, these just determine how many bytes an int takes up. The int takes up 4 bytes, while a short int will be halved to 2 bytes, and the long int doubled to 8 bytes. Like earlier, this has to do with historical reasons to conserve memory. An int is fine for most things, but if you need a large number (larger than 2 billion), use a long int (up to 18 quadrillion).

**signed** and **unsigned** have to do with if the variable can hold positive or negative values. Ints by default are **signed**, meaning they can hold either. However, if you need to make sure a number will not be negative, use the modifier **unsigned** to declare it as so. The **signed** keyword is utterly useless do to variables being signed by default, you will never have any reason to use it. 

These modifiers can be stacked, (eg, long unsigned int, signed short int, etc).

Thats about it for variables. In the coding section later ill demonstrate how to actually asign and use variables.

### Functions

