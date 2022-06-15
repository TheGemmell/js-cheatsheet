# JavaScript Cheatsheet

# Variable Declarations
~~`var` Declare a variable that can be changed later~~

`let` - Declare a variable that can be changed later

`const` - Declare a variable that can not be changed later
> there are some other differences between `var` and `let` to do with **scope** but we won't get into that for now.

# Operators

## Logical

`&&` and

`||` or

`!` not

## Comparison
`==` Loose Equal (Equal value)

`===` Strict Equal (Equal value && type)

`!=` Loose Not Equal (Not equal value)

`!==` Strict Not Equal (Not equal value || type)

`>` Greater Than

`<` Less Than

`>=` Greater Than || Equal To

`<=` Less Than || Equal To


## Arithmetic 
`+` Addition

`-` Subtraction

`*` Multiplication

`/`  Division

`%` Modulus (Returns the remainder of a division)


`**` Exponentiation (multiply to the power of)
***

# Data Types

## Primitive Types
1. `Number` Any number
2. `Boolean` Represented as True or False (1 or 0) 
3. `Null` Intentional absence of a value (It exists, but it doesn't have a value)
4. `Undefined` Absense of a value (it doesn't exist)
5. `BigInt` Used for storing numbers larger than 9,007,199,254,740,991
6. `String` Grouping of characters, aka text (letters, numbers, spaces, symbols, etc) 
7. `Symbol` Used for anonymouse, unique values. (Useful in complex, security-driven applications)


# Conditional Statements

## Falsy values 
1. 0
2. Empty strings like "" or ''
3. null which represent when there is no value at all
4. undefined which represent when a declared variable lacks a value
5. NaN, or Not a Number


# Loops
## For
```javascript
for (param1; param2; param3) {
    // Code block to be executed
}
```
`For` loops take in 3 parameters seperated with a semicolin `;` instead of the usual comma `,`

`param1` - executes when the loop starts

`param2` - the condition that must be met execute each loop

`param3` - executes every time the loop is iterated

### Example:
```javascript
for (let i = 0; i < 10; i++) {
    console.log(i)
}
```
The above example will log `i` to the `console` 10 times as `i` increases with every iteration
***

## While
```javascript
while (condition) {
    // Code block to be executed
}
```
`While` loops take in a `condition` and will loop until that condition is no longer true

> *_Be extremely careful with `while` loops, as they are extremely easy to get stuck in an infinite loop, this can crash the page and/or computer running it._

### Example

```javascript
let i = 0 // If we left out this line, it would never run!
while (i < 10) {
    console.log(i)
    i++ // If we forgot this, it would loop infinitely
}
```
The above example will run 10 times, as you can see, we need to declare the value of `i` outside the loop. Otherwise it would never start the loop, because JavaScript doesn't know what `i` means

If we were to forget to increment `i` after each iteration, it would run forever. Since the condition would never be false, as `i` would never get higher than `0`

