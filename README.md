# An Introduction to the C Programming Langauge

## Preface 
This project will hopefully help explain C.

Does not cover setup, use repl.it for simplicity.

Enjoy (:

## Some background knowledge

### Variable Typing

A type is quite simply the form of value a variable holds. It could be a number or decimal or a list, etc.
C is a statically typed language, so some clarification is needed first, especially for Python programmers

In Python, variables are dynamically typed. Variables can hold any sort of value, with no extra explanation
```
x = "hello world" // x is a string
y = [0, 1, 2, 3] // y is a list
z = lambda: print(x) // z holds a piece of code
```
And so on and so forth. However in C, variables must explicitly be given a type. 

The declaration is a little bit more involved: 
```
int x = 1; // an integer
float y = 3.14; // a floating point (decimal) value
char z = 'A' // a character
```
Once asigned a type, a variable holds only values of its type, and the type cannot change

While this may seem a little odd, it helps clarify what a variable is supposed to hold
```
int age = 15; // ages are whole numbers
float interest = 0.04; // while interest is usually a precentage
```
Takes a little bit to get used to.

### Variable Types

C has a very small amount of base types. They are as follows:
- int: whole numbers
- float: floating point decimal, holds up to 7 decimal digits
- double: double precision decimal (twice as large as a float, holding 15 decimal digits)
- char: quite literally a character

Expanding more on the char type, chars are actually numbers that hold a value representing a single character
C uses standard ascii encoding, which can be found [here](https://ascii-tables.com/) if your interested

And thats pretty much it. Howver, these types can have modifiers
