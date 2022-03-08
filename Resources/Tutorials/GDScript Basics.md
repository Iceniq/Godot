# [Introduction](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplusntro)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over how to approach taking this series.

### To summarize what’s in the video:

- The series is open to all programming levels; however, it was created with absolute beginners in mind

- Take lots of notes; I go over quite a lot

- Every video has a [github](https://github.com/Godot-Tutorials) project file you can download to practice what you’ve learned

- Don’t hesitate to ask me questions on the [youtube](https://www.youtube.com/channel/UCnr9ojBEQGgwbcKsZC-2rIg) comments section or

send me an email through the [contact form](https://godottutorials.com/contact)

- Have fun!

# [Data Types & Literal Values](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus0)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over data types and literal values in Godot GDScript.

Even though this is a more advanced topic, try your best to understand data types and literal values.

Game programming is all about manipulating literal values.

### What is a literal?

In programming, a literal is a value directly written in the source

code instead of being the result of some other expression (such as

referencing a variable or a constant).

Think of a literal as something you ‘literally’ provide in your script.

### What is a data type?

A data type is an attribute of data that tells the compiler/interpreter how the programmer intends to use the data.

Data types define the operations that can be done on the data, the

meaning of the data, and the way values of that type can be stored.

Some common data types include `Strings`, `Numbers/Integers`, `Floats`, `Booleans`, and `Null`

### Strings

Strings are a data type used in programming to represent text rather than numbers.

It is comprised of a set of characters that can contain spaces and numbers.

A string value is denoted by values inside the double quotation symbols `" "`.

- `"Hello World"` is a string value.

- `"I have 0 cats!"` is a string value.

- `"100"` is a string value.

- `"true"` is a string value.

- `"Null"` is a string value.

One thing to keep in mind is that you cannot do numerical calculations with string values.

`"1" + "1"` (strings) in programming is not the same as `1 + 1` (integers).

`"1" + "1"` will become the string value `"11"` whereas `1 + 1` will become the integer value 2.

### Integers/Numbers

An integer is a data type that represents some range of whole mathematical numbers.

In Godot GDScript, this range is between the values `-9223372036854775808` and `9223372036854775807`.

Integers are whole numbers. Some examples of whole numbers include `0`, `-100`, `911`.

Integers can be both positive, negative, and the number zero.

The most important aspect of an integer value is that it cannot have a decimal point (`.`).

If there is a decimal point in the number, then it is a float data type value.

### Floats

A float s a floating-point number, which means it is a number with a decimal point.

Float data types are used when precision in mathematical calculations are needed.

A float value is similar to an integer. It is a numerical value; the only difference is that a float value is a decimal number.

Some examples include `0.0`, `-100.0`, and `911.0`.

Notice that the only difference here versus their integer counterpart is the decimal point.

If it’s a whole number, then it’s an integer. If it has a decimal point, then it’s a float data type.

### Booleans

The boolean is a data type that has only one of two possible values.

Boolean values are denoted by the keywords `true` and `false`.

The keyword `true` numerically represent the values `1`,

while the keyword `false` numerically represents the value `0`.

### Null

The null data type is used to represent the absence of data.

The null value is denoted by the keyword `null`.

In GDScript, null is an empty data type that contains no information and cannot be assigned any other value.

# [Variables](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus-1)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over variables in Godot GDScript.

### What is a variable?

In computer science, a variable stores information to be referenced to and manipulated in a computer program.

### How to write a variable?

In GDScript, you define a variable using the `var` keyword.

You need to have 4 crucial things in a single line of code to write a variable.

1. Use the `var` keyword to signify the creation of a variable

2. Immediately following the `var` keyword, come up with a name for the newly created variable

3. Use the `=` symbol to assign a value to your variable. The `=` character is also called the assignment operator

4. Lastly, after the `=` character, assign a literal value to your variable.

In the following example, the values `a`, `b`, and `c` are variables:

```csharp
var a = "hello world"

var b = 100

var c = 9.5
```

### Do I need to always assign a value to a newly created variable?

The answer is, no, you don’t have to.

A variable without a value is called an uninitialized variable.

This means that a variable is declared, but no value has been assigned to it.

```csharp
var a

var b

var c
```

The variables `a`, `b`, `c` are variables

### How to write a typed variable?

Godot allows you to write typed variables.

This limits a variable to only contain values of a specific data type.

To create a typed variable, all you have to do is use the colon symbol (`:`) followed by the data type.

```csharp
var a: int = 100

var b: String = "Hello world"

var c: float = 98.9

var d: bool = true
```

- Variable `a` can only be assigned integer values.

- Variable `b` can only be assigned string values.

- Variable `c` can only be assigned float values.

- Variable `d` can only be assigned boolean values.

You can also infer the data type by the value being assigned to the variable:

```csharp
var a := 100

var b := "Hello World"

var c := 98.9

var d := true
```

- Variable `a` can only be assigned integer values.

- Variable `b` can only be assigned string values.

- Variable `c` can only be assigned float values.

- Variable `d` can only be assigned boolean values.

In Gdscript, values assigned to a typed variable must have a compatible type.

If you need to coerce a value to be a particular type, you can use the casting operator keyword `as`.

```csharp
var text: String = 100 as String

var num: int = "100" as int

var numFloat: float = 100 as float
```

- Variable `text` has the value of 100 transformed into a string value.

- Variable `num` has the value “100” transformed into an integer value.

- Variable `numFloat` has the value of 100 converted into a float value.

# [Life Cycle & Reference Counting](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus-2)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over Life Cycles & Reference Counting in

General Programming. I made the unfortunate mistake of mistaking how

Godot handles memory management.

The video’s information is still accurate for the following examples in the C language and the python language.

# [Operators & Operands](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus2)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over operator & operands in Godot GDScript.

### What are operators?

Operators allow you to “operate on” or manipulate variables/constants.

Operators are symbols (`=`, `<`, `+`, etc) that instruct the program to perform a task.

### What is an operand?

An operand is a variable, constant, or expression that acts upon the operator.

```csharp
var a = 1 + 2
```

In this example, the integers `1` and `2` are **operands**. The `+` symbol is the **operator**.

The operator instructs the program to add the numbers 1 and 2 together.

On top of that, the `=` symbol is the assignment operator. It instructs everything to the left of the symbol

to be assigned to the variable on the left side of the `=`.

### Arithmetic Operators

| Operators | Description |

| --- | --- |

| +   | Addition Operator |

| -   | Subtraction Operator |

| *   | Multiplication Operator |

| /   | Division Operator |

These operators are self-explanatory.

You will add, subtract, multiply, and divide operands together.

```csharp
1 + 2 # addition operand

1 - 2 # subtraction operand

1 * 2 # multiplication operand

1 / 2 # division operand
```

### Relational Operators

Relational operators are used when you want to compare operands.

| Operators | Description |

| --- | --- |

| ==  | Equal to operator |

| !=  | Not equal to operator |

| >   | Greater than operator |

| >=  | Greater than or equal to operator |

| <   | Less than operator |

| <=  | Less than or equal to operator |

When using relational operators, the value returned to you is a boolean value `true/false`.

If the relational statement is satisfied (if it is true), then a `true` value is returned.

If a relational operator is not satisfied (if it is false), then a value of `false` is returned.

```csharp
1 == 2 # returns false

1 != 2 # returns true

1 > 2 # returns false

1 >= 2 # returns false

1 < 2 # returns true

1 <= 2 # returns true
```

Keep in mind the values returned from the greater/less than operator.

```csharp
2 > 2 # returns false

2 < 2 # returns false

2 >= 2 # returns true

2 <= 2 # returns true
```

### Logical Operators

Logical operators are used when you want to compare the truth/false values of an operand.

You will usually use logical operators inside of if statements and while $loops$.

| Operators | Description |

| --- | --- |

| && (AND) | AND Operator |

| \\| (OR) | OR Operator |

| ! (NOT) | NOT Operator |

- You use the `&&` operator to check if two operands are true

- You use the `||` operator to check if one out of two operands are true

- You use the `!` operator to check if the operand is false

```csharp
true && true # returns true

false && true # returns false

false || true # returns true

false || false # returns true

!false # returns true

!true # returns false
```

# [Constants](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus3)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over constant variables in Godot GDScript.

### What are constant variables

A constant - also referred to as a constant variable - is a value

that cannot be changed or altered by the application during runtime.

Put into simpler terms, a constant is a value that can never change.

### How to declare a constant in GDScript

To declare a constant, all you have to do is use the `const` keyword.

```csharp
const neverChanges = 100
```

In this case, you have a constant value called `neverChanges`, and it is assigned the value 100.

Like a variable, you can also declare a constant as a typed value. Still, it is redundant since the value can never change.

```csharp
const neverChanges: int = 100

const neverChangesAgain := 100
```

If you ever try to change the value, an error will be thrown.

```csharp
const neverChanges = 100

neverChanges = 99 # throws an error
```

### What are the pros of using constant values

Constant values give you three benefits:

1. Readable Code

2. Easier Debugging

3. Saves you time when editing

### Aren’t constants the same as literals?

You can use literals instead of constants. To the compiler/program, it doesn’t make a difference.

However, for the sake of readability, it is easier to use constants.

Here is an example:

```csharp
var playerSpeed = 100

var laserSpeed = 100

var bomerangSpeed = 100

# imagine the speed value of 100 is in many places
```

This may seem alright when dealing with a few lines of code. However,

imagine that the speed with a value of 100 is in many places.

Now imagine yourself trying to find and edit your literal value 100 when you decide that the speed value should be changed to `99`.

It would be easier to use constants.

```csharp
const SPEED = 100

var playerSpeed = SPEED

var laserSpeed = SPEED

var bomerangSpeed = SPEED
```

Editing one line of code, in this case, `const speed = 100`, will update the values of many lines of code that uses the

speed constant value.

### Constant best practices

Use constants when you want to declare a value that you know will never change in your game or application’s entire life cycle.

Some examples of game values that may never change (depends on the game):

- player height

- player speed

- player attack damage

On top of that, ensure that the naming convention of constants' names is visually different from variables.

```csharp
const SPEED = 100 # SNAKE_UPPERCASE

const NORMAL_SPEED = 50 # SNAKE_UPPERCASE

var player_health = 100 # snake_lowercase
```

In the sample script, notice how constant values are all snake case

uppercase. That means all words are separated by underlines, and all

letters are in the uppercase format.

Compare that to the variable naming convention of snake lowercase.

Meaning all words are separated by underscores, and all letters are

lowercase.

You are free to choose your naming conventions.

Just make sure that constant names look different than variable names.

This makes it easy for you to see which variable names are free to change and which constant variables are not open to change.

# [Comments](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus4)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over comments in Godot GDScript.

### What is a comment?

A comment is a programmer-readable explanation or annotation in the source code of a computer program in computer programming.

They are added to make the source code easier for humans to understand and are generally ignored by compilers and interpreters during runtime.

### How to write comments in GDScript

You can use the `#` symbol followed by your comment text.

You can use the triple quotation marks for opening and closing your comments `"""`. Keep in mind that the compiler will interpret this as a multi-line string value.

```csharp
# This is a single line comment

"""
This is a multiline comment.
This is a multiline comment.
This is a multiline comment.
"""
```

### Types of comments

There are 4 different types of comments you may find yourself using:

- Methodology Description
- Meta-Data
- Debugging
- Code Description

### Methodology Description

Methodology comments can be used to explain the code you are using rather than the clarification of its intent.

For example, in your code for a sorting algorithm, you may use a methodology comment to explain why you used the insertion sort algorithm instead of the quick sort.

```csharp
"""
Quicksort turned out to be slower than insertion sort for our list. For this reason, I went with insertion sort.
"""
```

### Meta-Data

These comments are at the top of a script file.

They will include things like the company name, author, file name, etc.

You will typically see this sort of comment on open source code.

```csharp
"""
This file is part of:
Godot Game Engine
https://godotengine.org
***********************
Copyright (c) 2007 -2021 Juan Linietsky, Ariel Manzur
"""
```

### Debugging

Debugging comments are used when you want to apply brute force debugging techniques on your code.

An example would be commenting out print statements (which print things to console).

```csharp
if(x < 10):
    # print(x)
    x = x + 1
```

### Code Description

Generally used o make others understand the intent of a line of code.

This type of comment should be used only when needed.

Sometimes if used, it is a sign of lousy variable naming convention.

The following is an example of a Code Description comment.

```csharp
# Player health
var x = 100
```

In this case, it is a lousy use of Code Description. You can do a better job of describing your code through its variable name.

```csharp
var player_health = 100
```

You can do even better by expressing what values you’d like your variable to have

```csharp
var player_health: int = 100
```

### When to use comments

There is a saying:

> Code tells you how, and comments tell you why

Try to use naming conventions to improve your code readability.

When you have reached that limit, use comments to explain the rationale of your code.

# [Conditional Statements (if/elif/else)](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus6)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over conditional statements (if/elif/else).

### Definition

In programming, conditional statements are features of a programming language, which perform different computations or actions depending on whether a programmer-specified boolean condition evaluates to true or false.

In layman’s terms, sometimes programmers would like to do different code actions based on other decisions or results we get from code.

### What types of conditional statements does GDScript have?

There are two different ways you can handle conditional statements in GDScript:

- if/elif/else statements
- match statements

### The if keyword

Use the `if` keyword to specify a block of code that runs if a condition is true:

```csharp
if 2 > 1:
    # run everything inside the block of code
```

If a condition is false, the block of code is skipped.

```csharp
if 2 < 1:
    # Block of code never runs
```

### The else keyword

Use the `else` keyword to run a block of code if the if statement condition is false:

```csharp
if 2 < 1:
    # Block of code never runs
else:
    # Block of code runs
```

In this case, because the integer value 1 is never greater than 2, the else statement will always run.

### The elif keyword

Sometimes we want to test against multiple conditions before reaching an else keyword.

To do that, we use the `elif` keyword.

The `elif` keyword runs whenever the condition inside the if statement turns out false.

```csharp
if 2 < 1:
    # Block of code never runs
elif 2 > 1:
    # Block of code runs
```

You are also able to chain multiple elif keywords together:

```csharp
# An if statement chain
if 1 < 2:
    # block of code
elif 1 < 3:
    # block of code
elif 1 < 4:
    # block of code
else:
    # run code
```

Just keep in mind that you can only have one `if` keyword and one `else` keyword in a single if statement chain.

### Guess what happens here

```csharp
var health: int = 100

if health >= 100:
    print("Full Health")

elif health > 60:
    print("Health is Good")

elif health > 30:
    print("Health is low")

elif health >= 1:
    print("Health is dangerously low")

else:
    print("Health is depleted")
```

# [While Loop](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus7)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over while loops in Godot GDScript.

### While keyword

With the `while` keyword, you can run the block of code for as long as the while loop’s condition continues to be true.

```csharp
var x: int = 0
while x < 10:
    print(x)
    x = x + 1
```

### Break keyword

With the `break` keyword, you can get out of a loop.

```csharp
var x: int = 0
while x < 10:
    break
    # you don't get a chance to run the rest of the code block
    print(x)
    x = x + 1
```

### Infinite Loop

An infinite loop, also referred to as an endless loop, lacks a functional exit and repeats indefinitely.

### Types of Infinite Loops

There are 3 different types of loops you may find yourself using:

- Fake Infinite Loop
- Intended Infinite Loop
- Unintended Infinite Loop

### Fake Infinite Loop

Fake infinite loops give the impression of an endless loop, but when you look closely, they have an exit:

```csharp
var x: int = 0
while true:
    print("Hello World")
    break # an exit, without this the loop would run forever
```

In the example above, it looks like it would run indefinitely; however, on closer inspection, you will see that there is a break keyword; therefore, the block of code will run only once.

### Intended Infinite Loop

An intended infinite loop is an endless loop where the programmer intentionally writes a loop where they don’t want it to end.

An example of an intended infinite loop would be the game loop.

In game programming, your code is always running an intended infinite loop.

You only ever stop the loop when a game user exits the game.

### Unintended Infinite Loop

As the name suggests, this type of loop is one where the programmer makes a mistake.

Try your best not to make this type of infinite loop.

# [For Loops](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-gdcplus8)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over for loops in Godot GDScript.

### What is a for loop?

A for loop is a control flow statement that allows code to be executed repeatedly.

This type of loop allows for the enumeration (iteration) of sets of items other than a sequence of numbers.

For starters, you can loop through literal integers:

```csharp
for x in 10:
    print(x)
```

The numbers 1 - 10 will print to the console in the Godot application in the script above.

```csharp
var arrayExample = [10,20,30]
for x in arrayExample:
    print(x)
```

In the script above, the numbers 10, 20, and 30 will print to the console.

### When to use a for loop

You will use a for-loop when you want to have an array or dictionary item you’d like to iterate over.

# [Match Statement](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-09)

Hello and welcome to the GDScript fundamental tutorial series.

In this episode, I go over coding match statements in Godot GDScript.

### What is a match statement?

A match statement, just like a case statement, is a type of selection control mechanism used to allow the value of a variable or expression to change the control flow of program execution in search and map.

Basically, you use a variable to ‘match’ a pattern and execute the code inside the match statement.

```csharp
# Example of a match statement chain

var health: int = 1

match x:
    1:
        # If health == 1, run this block of code
    _:
        # If nothing matches, run this block of code
```

### Types of match patterns

- Constant Pattern
- Variable Pattern
- Wildcard Pattern
- Binding Pattern
- Array Pattern
- Dictionary Pattern
- Multiple Patterns

### Constant Pattern

A constant pattern is when you use a primitive/literal data type.

These would include integers, floats, booleans, strings, etc.

When matching string values, keep in mind that they are case sensitive.

```csharp
var health: int = 1

match health:
    1:
        # Constant Pattern Block
    "Hello":
        # Constant Pattern Block
    2.03:
        # Constant Pattern Block
    true:
        # Constant Pattern Block
```

### Variable Pattern

With GDScript, you can use variables as a match pattern.

```csharp
var health: int = 1
var matchPatternOne: int = 1

match x:
    matchPatternOne:
        # Variable Pattern Block
```

### Wildcard Pattern

A wildcard pattern is when you use the underscore symbol as a match pattern `_`.

You use the wildcard pattern when you want to match everything.

It can also be thought of as a “default” block statement, meaning it will always run when all other match patterns fail.

Since the match patterns run in chronological order, it is best to use the wildcard pattern as the last pattern in your match statement chain.

```csharp
var health: int = 1

match x:
    _:
        # Wildcard Pattern Block will always run when everything fails
```

### Binding Pattern

A binding pattern catches everything just like the wildcard pattern. The difference is the binding pattern assigns the value acquired into a variable that can be used inside the binding pattern match block.

```csharp
var health: int = 1

match x:
    var matchValue:
        # Binding Pattern Block, matchValue will equal the match variable
        # matchValue = x
```

### Array Pattern

You can use arrays as a match pattern.

Every single element in the array is a match pattern in itself.

You can also use sub-patterns inside your array. The `..` is a sub-pattern. Using the `..` makes the array an open-ended array.

Arrays patterns are tested in the following way:

1. The length of the array is tested. The match fails if the array lengths are not the same. Unless you use the `..` sub-pattern.

2. The match array is tested against the array pattern. If a single element is different, then the pattern fails.

```csharp
var health: int = [1,2,3]

match x:
    []:
        # only an empty array will match
    [1,2]:
        # An array of only [1,2] will match
    [1,2,..]:
        # An array with the first and second elements being [1,2] will match
        # The array can have any other value after the third element and still match
```

### Dictionary Pattern

A dictionary pattern is used to test against dictionaries.

Sub-patterns such as `..` can also be used.

Dictionary patterns are tested in the following way:

1. The length of the dictionary is tested. The match fails if the dictionary lengths are not the same. Unless you use the `..` sub-pattern.

2. Key and values are tested. If a single element is different, then the pattern fails.

```csharp
var health: int = {"key": "value", "key2", "value2"}

match x:
    {}:
        # only an empty dictionary will match
    {"key": "value"}:
        # A dictionary of {"key": "value"} will match
    {"key": "value", ..}:
        # A dictionary of {"key": "value"} will match followed by another key/value pair
```

### Multiple Pattern

You can specify multiple patterns as long as they are separated by commas:

```csharp
var health: int = 3

match x:
    1,2,3,4,5:
        # Matches any variable that has an integer in the range of 1-5
```

# [Match Statement Use Case](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-9-1)

The match statement will help you avoid and/or fix massive `if` statement chains

### Godot Tutorials Resources

- [Youtube](https://www.youtube.com/channel/UCnr9ojBEQGgwbcKsZC-2rIg)

- [Twitter](https://twitter.com/GodotTutorials)

- [Reddit](https://www.reddit.com/user/Godot_Tutorials)

- [Github](https://github.com/Godot-Tutorials)

- [Trello](https://trello.com/b/TAHIZJ9D/godot-game-tutorials)

# [Arrays](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-10)

Arrays are a collection of values/items stored together.

In GDScript, arrays can contain values of different data types.

```csharp
var example = [] # an empty array
var anotherExample = [1, "hello", true] # an array with different data types
```

You are able to retrieve a single element from the array:

```csharp
var example = [10, 20, 30]
var firstElement = example[0] # 10
var secondElement = example[1] # 20
var thirdElement = example[2] # 30
```

### Length of an Array

To get the length of an array, use the `size` method:

```csharp
var example = [ 1,2,3 ]

var length = example.size()
print(length) # 3
```

### Sub Arrays

You can have arrays inside of arrays. These are called sub-arrays.

```csharp
var subArray = [ [1,2], [9,10] ] # an empty array

# Get a value from the first subarray
var subarrayValueOne = subArray[0][0] # 1
var subarrayValueTwo = subArray[1][1] # 10
```

### Push and Pop Methods

To push a value to either the front or back of an array, use the push method:

```csharp
var example = [ 1,2,3 ] # an empty array

# Get a value from the first subarray
example.push_front(0) # example = [0,1,2,3]
example.push_back(4) # example = [0,1,2,3,4]
```

To pop a value out of an array, you can use the pop method:

```csharp
var example = [ 1,2,3 ] # an empty array

# Get a value from the first subarray
example.pop_front() # example = [2,3]
example.pop_back() # example = [3]
```

### Empty an array

There are a few ways to clear an array:

1. You can assign an empty array

```csharp
var example = [ 1,2,3 ]

example = []
```

2. You can resize an array using the `resize` method

```csharp
var example = [ 1,2,3 ]

example.resize(0)
```

3. You can clear an array using the `clear` method

```csharp
var example = [ 1,2,3 ]

example.clear()
```

### Duplicate an array

In Godot, if you try to pass an array to another variable, an issue occurs.

The issue is that two variables will have access to the same array values.

```csharp
var example = [ 1,2,3 ]

var anotherArray = example # anotherArray = [1,2,3]

anotherArray.push_front(4)

print(example) # [1,2,3,4]
```

To avoid this issue, you will need to implement either a deep copy or a shallow copy.

### Shallow Copy

A shallow copy copies the array except for sub-arrays.

This means that all nested arrays and dictionaries will be shared with the original array.

A shallow copy uses the `duplicate` method with the false value passed inside the parentheses.

```csharp
var example = [ 1,2,3, [1,2] ]

var anotherArray = example.duplicate(false) # anotherArray = [1,2,3,[1,2]]

anotherArray.push_front(4)

print(example) # [1,2,3,[1,2]]

anotherArray[3][0] = 100

print(example) # [1,2,3,[100,2]]
print(anotherArray) # [1,2,3,[100,2],4]
```

### Deep Copy

A deep copy copies the array, including sub-arrays.

This means that all nested arrays and dictionaries will not be shared with the original array.

To do a deep copy, use the `duplicate` method with the value `true` passed inside the parentheses.

```
var example = [ 1,2,3, [1,2] ]

var anotherArray = example.duplicate(true) # anotherArray = [1,2,3,[1,2]]

anotherArray.push_front(4)

print(example) # [1,2,3,[1,2]]

anotherArray[3][0] = 100

print(example) # [1,2,3,[1,2]]
print(anotherArray) # [1,2,3,[100,2],4]
```

# [Arrays & Dynamic Memory Address](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-10-1)

### Godot Tutorials Resources

- [Youtube](https://www.youtube.com/channel/UCnr9ojBEQGgwbcKsZC-2rIg)

- [Twitter](https://twitter.com/GodotTutorials)

- [Reddit](https://www.reddit.com/user/Godot_Tutorials)

- [Github](https://github.com/Godot-Tutorials)

- [Trello](https://trello.com/b/TAHIZJ9D/godot-game-tutorials)

# [Strings (Basics of Memory)](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-10-2)

### Resources

Github Project:

- [Link to Github Project](https://github.com/Godot-Tutorials/Strings)

### Godot Tutorials Resources

- [Youtube](https://www.youtube.com/channel/UCnr9ojBEQGgwbcKsZC-2rIg)

- [Twitter](https://twitter.com/GodotTutorials)

- [Reddit](https://www.reddit.com/user/Godot_Tutorials)

- [Github](https://github.com/Godot-Tutorials)

- [Trello](https://trello.com/b/TAHIZJ9D/godot-game-tutorials)

# [Enums](https://godottutorials.com/courses/introduction-to-cplus/godot-tutorials-cplus-11)

Enums, also referred to as enumerations, are a data type that contains a fixed set of constants.

### Global Enums

```csharp
enum {LEFT, RIGHT, UP, DOWN}

# Same as writing
const LEFT = 0
const RIGHT = 1
const UP = 2
const DOWN = 3
```

### Local Enums

```csharp
enum MOVE_SET {LEFT, RIGHT, UP, DOWN}

MOVE_SET.LEFT # 0
MOVE_SET.RIGHT # 1
MOVE_SET.UP # 2
MOVE_SET.DOWN # 3
```

# [Dictionaries](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-12)

Dictionaries, also referred to as a key-value store, are associative containers that contain values referenced by keys.

```csharp
var simpleDictionary = {"name": "John"}
```

In the code above, the key `name`, while the value is `"John"`

You are also able to use other datatypees besides strings as keys:

```csharp
var integerDictionary = {1: "John"}
var floatDictionary = {2.13: "Jane"}
var booleanDictionary = {true: "Sarah"}
```

### Accessing Dictionaries

```csharp
# Create Dictionaries
var simpleDictionary = {"name": "John"}
var integerDictionary = {1: "Jane"}
var floatDictionary = {2.13: "Josh"}
var booleanDictionary = {true: "Sarah"}

# Retrieve values
var getJohn = simpleDictionary["name"] # "John"
var getJane = integerDictionary[1] # "Jane"
var getJosh = floatDictionary[2.13] # "Josh"
var getJohn = booleanDictionary[true] # "Sarah"

# You can use dot notation if retrieving string keys
var getJohnAgain = simpleDictionary.name # "John"
```

### Assigning Values to an Existing Key

```csharp
var simpleDictionary = {"name": "John"}

# One way
simpleDictionary["name"] = "Jane"

# Another way
simpleDictionary.name = "Jane Doe"
```

### Creating New Key-Value Pair

```csharp
var simpleDictionary = {"name": "Jane"}

simpleDictionary["birthdate"] = "December 2020"

simpleDictionary.age = 0
```

### Comparing Dictionaries key-value pairs

If you compare dictionaries with a comparison operator, you will return false even if the
dictionaries compared are exactly the same:

```csharp
var simpleDictionary = {"name": "Jane"}
var sameDictionary = {"name": "Jane"}

if(simpleDictionary == sameDictionary):
    # Block of code never runs
```

To get the desired results when coparing dictionaries, use the `hash` method:

```csharp
var simpleDictionary = {"name": "Jane"}
var sameDictionary = {"name": "Jane"}

if(simpleDictionary.hash() == sameDictionary.hash()):
    # Block of code runs
```

### Delete a key-value pair

To delete a key-value pair, use the `erase` method:

```csharp
var simpleDictionary = {"name": "Jane"}

simpleDictionary.erase("name")
```

# [Functions](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-13)

A function is a block of organized and reusable code used to perform a single, related task/action.

Functions are also referred to as methods, procedures, or sub-routines.

On top of that, functions are always part of a class and can return back values if needed.

### Simple Function

```csharp
func simpleExample():
    pass
```

In this case, the `simpleExample()` funciton does nothing.

The `pass` keyword does nothing except preventing the compiler from showing the empty function soft error.

The `pass` keyword can also be used in loops to avoid the empty loop error.

### Function with Parameters

You can pass values into a function through the function’s parameter (the parenthesis):

```csharp
func simpleExample(parameter):
    pass
```

### Function with Specific Data Type Parameters

You can also force a single data type onto a parameter value:

```csharp
func simpleExample(parameter: String):
    pass
```

In this case, our `simpleExample` function parameter can only take in string values.

You can also set the default value of a parameter:

```csharp
func simpleExample(parameter := "default value"):
    pass
```

In this case, we would like our parameter to take in only string 
values, and if none is provided the default value will be the literal 
string “default value”.

Keep in mind that the `:=` infers the data type.

### Function with Specified Return Type

You can declare what type of value is returned from the function using the `->` symbol and the `return` keyword:

#### void

The `void` data type specifies that your function does not return back anything.
When using the `void` data type, you do not have to provide the `return` keyword.

```csharp
func simpleExample() -> void:
    return
```

#### int

```csharp
func simpleExample() -> int:
    return 10
```

#### float

```csharp
func simpleExample() -> float:
    return 2.13
```

#### bool

```csharp
func simpleExample() -> bool:
    return true
```

### Function Name Best Practices

Stay consistent with naming your functions.

I use camelCases for small projects.

```csharp
# camelCase

func simpleExample() -> bool:
    return true
```

For bigger ones, consider using snake_case:

```csharp
# snake_case

func simple_example() -> bool:
    return true
```

# [Scope](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-14)

The scope is the region of a computer program where a name binding is
 valid. Name binding is just a fancy word for saying “variables”.

Scopes can vary in range in a programming application.

These can be from small for loops and if statements to entire classes.

### Levels of Scope

- Global Scope
- Class/File/Module Scope
- Function Scope
- Code Block Scope

#### Global Scope

Global scope is a class, variable, or function that can be used anywhere in the
Godot Application.

An example would be the Node class:

```csharp
extends Node

# The rest of your class
```

#### Class Scope

A class scope is a variable or function that can be used anywhere in the class file.

```csharp
extends Node # Global Scope Class Name Node

# Class variables that can be used anywhere in the class file
var health: String = 100
var speed: float = 10.0
```

#### Function Scope

A variable/value that can only be used inside of a function

```csharp
extends Node # Global Scope Class Name Node

#Class Scope
var health: String = 100
var speed: float = 10.0

func example():
    # variable functionVariable can only be used inside of the function `example()`
    var functionVariable = 10
```

#### Code Block Scope

A variable/value that can only be used inside of a code block.

Example fo code blocks would be the if statement, match statement, for & while loops, etc:

```csharp
extends Node # Global Scope Class Name Node

# Class Scope
var health: String = 100
var speed: float = 10.0

func example():
    # Function Scope
    var functionVariable = 10
    if(true):
        # Code Block Scope
        # variable message exists only inside this one if statement
        var message = "Hi!"
        print(message)
```

# [Classes](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-15)

Classes describe an aggregate of ta fields such as variables and defines the operations, such as methods.

Think of a class as a blueprint for creating objects, with initial value states, and implementation behavior.

In GDScript, by default, all script classes are unnamed classes.

This means you can only reference a class by its relative path.

#### Absolute Path

```csharp
# Absolute Path on Windows
"C:\Data\Filepath"
```

#### Relative Path

```csharp
# Relative Path through GDScript
"res://path/to/file.gd"
```

### Basic Class Format

Use the `extends` keyword in a class file to let Godot know which Global Godot class
your script file inherits from.

The `extends` keyword determines what Node functions are available to you.

You can learn more about the Godot Global Classes in the Godot Basics Series.

Classes can also have class/member variables and functions.

Class/member variables are available in the entire class file.

```csharp
# Example.gd
extends Node2D

var playerHealth: int = 100
var playerSpeed: float = 5.0

func getPlayerHealth() -> int:
    return playerHealth
```

If you omit the `extends keyword`, your class will inherit from the `Reference` global class:

```csharp
# Example.gd
# Extends from Global Reference Class

var playerHealth: int = 100
var playerSpeed: float = 5.0

func getPlayerHealth() -> int:
    return playerHealth
```

### Naming a Class

Use the `class_name` keyword to name a class and add it to the global scope.

The newly created class will be available in other .gd files and scenes in Godot.

```csharp
#Player.gd

extends Node2D

class_name Player

# class variables and functions
```

```csharp
#Scene.gd

extends Node2D

var playerInstanceObject = Player.new() 
```

### Class Inheritance

A GDScript class can inherit from the following:

- Global Class
- Another Class
- An Inner Class

### Inner Class

An inner class is a class inside of a class.

```csharp
extends Node

# class instance object
var object = InnerClass.new()

func _ready():
   var getInnerValue = object.getA()
   print(getInnerValue)

class InnerClass:
   #member variables
   var another = 100

   func getAnother():
      return another
```

### Virtual Method

A virtual method is a method that can be redefined in a derived class.

It is used when a method’s basic functionality is the same, but sometimes more is needed in the derived class.

# [Class Objects](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-16)

A class object is an instance of a class. A class object can also be 
referred to as a class instance, instanced object, or class object.

```csharp
#Player.gd

extends Node2D

class_name Player

# class variables and functions
```

```csharp
#Scene.gd

extends Node2D

var playerInstanceObject = Player.new() 
```

### Class Constructors

The class constructor is a particular function in which it is called every time a class object is created.

You define a class constructor using the `_init()` method:

```csharp
#Player.gd

extends Node2D

class_name Player

var playerHealth: int

# Class Constructor
_init():
    playerHealth = 100
```

```csharp
#Scene.gd

extends Node2D

var playerInstanceObject = Player.new() 
print(playerInstanceObject.playerHealth) # 100
```

You are also able to pass arguments into the constructor as well:

```csharp
#Player.gd

extends Node2D

class_name Player

var playerHealth: int

# Class Constructor
_init(startingHealth:int = 100):
    playerHealth = startingHealth
```

```csharp
#Scene.gd

extends Node2D

var playerInstanceObject = Player.new(200) 
print(playerInstanceObject.playerHealth) # 200
```

# [Class Inheritance](https://godottutorials.com/courses/introduction-to-csharp/godot-tutorials-csharp-17)

Class inheritance is a mechanism where you can derive a class from another class
for a hierarchy of classes that share a set of attributes and methods

To inherit from a class, use the `extends` keyword:

```csharp
# Animal.gd
extends Node2D # Inherits from the Global Node2D class

class_name Animal
```

```csharp
# Horse.gd
extends Animal # Inherits from the Global Node2D class

class_name Horse
```

In this case, the Animal class is called a superclass, while the Horse class is called the
subclass.

When a subclass inherits from a superclass, the subclass gets all the functions and class
variables of the superclass.

```csharp
# Animal.gd
extends Node2D # Inherits from the Global Node2D class

class_name Animal

var health: int = 100

func getHealth() -> int:
    return health
```

```csharp
# Horse.gd
extends Animal 

# Horse class has the health variable and the getHealth() method

class_name Horse

func newlyCreatedFunction() -> void:
    print(getHealth()) # 100
```

```csharp
# Animal.gd
extends Node2D # Inherits from the Global Node2D class

class_name Animal

var health: int = 100

func getHealth() -> int:
    return health
```

```csharp
# Horse.gd
extends Animal 

# Horse class has the health variable and the getHealth() method

class_name Horse

func newlyCreatedFunction() -> void:
    print(getHealth()) # 100
```

### Overriding a Superclass Function

You can override a superclass function by merely writing out the function in the subclass.

```csharp
# Animal.gd
extends Node2D # Inherits from the Global Node2D class

class_name Animal

func attack() -> void:
    print("Animal Attacks")
```

```csharp
# Horse.gd
extends Animal 

# Horse class has the health variable and the getHealth() method

class_name Horse

func attack() -> void:
    print("Horse Attacks") # Override function attack()
```

### Why is using inheritance necessary?

Inheritance allows for cleaner code, and it makes it easier for us to define classes.

Basically, you use inheritance when you want to reuse a class.

# [Classes as a Data Type](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-18)

A data type is an attribute of data that tells the compiler or interpreter how the programmer intends to use the data.

In Godot, GDScript classes are reference types (objects).

```csharp
var example: Node2D = Node2D.new() # variable example is a Node2D data type
```

You are also able to cast data types:

```csharp
var example: Node = Node2D.new() as Node # cast Node2D instanced object as Node
```

# [Duck Typing](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-19)

In programming, duck typing is a type system used in dynamic 
programming languages. The type or class of an object is less important 
than the method it defines.

With duck typing, you check if a class has a given method or attribute.

### Why is it called Duck Typing?

It comes from the saying:

> If it walks like a duck and quack likes a duck, then it must be a duck

Basically in the context of the program, as long as a class has the exact name of the function; we neither care
what the function specifically does nor do we care what class the specific function comes from.

### The `Is` Keyword

For duck typing and checking for null values, we will need to use the `is` keyword.

The `is` keyword is used to check the data type of a given object and returns a boolean value:

```csharp
5 is int # true
Frog is Animal # Does the Frog Class inherit from the Animal Class and is not empty?
```

### Example of Duck Typing

```csharp
# Animal Class

extends Node
class_name Animal

func fly():
   print('Animal flies')
```

```csharp
# Duck Class

extends Animal
class_name Duck

func fly():
   print('this duck flies')
```

```csharp
# Circle Class

extends Node
class_name Circle

func fly():
   print('Circles are flying???')
```

```csharp
# Node Class

extends Node2D

var animal = Animal.new()
var duck = Duck.new()
var circle = Circle.new()

# No Type Safety
"""
In this case we can pass it in everything and the function call will work
as long as the class object has that specific function name

letItFly(animal)
letItFly(duck)
letItFly(circle)
"""
func letItFly(flyingObject):
   flyingObject.fly()


# With Type Safety
"""
But what if we want type safety?
Say we only want Classes and Sub-Classes of the 'Animal' class???
"""
func animalFlies(animalObject: Animal):
   animalObject.fly() # comes with auto complete


"""
The problem is that an error will be thrown if the class is a null value

For Example:
   var nullObject: Animal # Null Instantiation w/ type safety

In this case nullObject will make it through the animalFlies() method without warning.
The game will crash when a null object tries to call the 'fly()' because it does not exist
on a null object

In this case we have to check that null values are not sneaking through
"""

# Check for the objects casted as Nulls
# var nullObject: Animal # casted as null but will make it through this function regardless
func animalFliesSafely(animalObject: Animal):

   # Option 1
   if animalObject == null:
      print('object/value does not fly')
      return

   # Option 2
   if (animalObject is Animal) == false:
      print('Animal Class not part of Inheritance Chain')
      return

   # Do whatever you want; you're an animal!
   print('continue on ;)')
   animalObject.fly() # without a null check, throws an error if null
```

### [Static Functions](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-20)

A static function is a member function of a class that can be called even when an object has not been initialized.

A static class cannot access any variables of its class except for static variables.

> Godot GDSCript does not have static variables.

You do not need to create a class instance to use a static function.

It’s best to use static functions when you don’t depend on any class members (variables).

```csharp
# Animal Class
extends Node2D

class_name Animal

static func printHi() -> void:
    print("Hello!")
```

```csharp
# Another Class

extends Node2D

# Inside of some function
_ready():

    # You do not need to instantiate the animal class in order to use printHi()
    Animal.printHi() # prints "Hello" to console
```

# [Export Keyword](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-21)

In Godot, class members can be exported to the Godot application using the `export` keyword.

A benefit of using the `export` keyword is that it’s easier to edit the values
of member variables.

```csharp
export var example = "Hello!"
```

The variable example will now be viewable in the Godot Application.

#### Export with Data Type Safety

```csharp
export(String) var example
```

The value will default to an empty string:

```csharp
export(int) var example
```

The value will default to `0`.

#### Export with Enumeration

```csharp
export(int, "Up", "Down") var example
```

The choices available are up or down, and the value will default to `0`.

#### Export with Integer Range

```csharp
export(int, 20) var example
```

You can input a value between 0 - 20

```csharp
export(int, 10, 20) var example
```

You can input a value between 10 - 20

# [Setters & Getters](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-22)

In programming, setters and getters are functions used to control the
 access of variables. They are quite useful when creating classes.

For each member variable, a getter function will return the variable value.
The setter function will update or “set” a value to a member variable.

To create a setter/getter method, use the `setget` keyword followed the name
of the setter and getter method.

`var <variable name> = <assignment value> setget <setter name> , <getter name>`

A Basic Getter/Setter Function:

```csharp
extends Node
class_name Human

# Both a setter & getter method established
var uniqueName = "John" setget setFunction, getFunction

func setFunction(param1):
   uniqueName = param1

func getFunction():
   return uniqueName
```

You are also able to pick and choose whether a member variable will only use a setter
or getter method.

To create only a setter method for a variable:

```csharp
extends Node
class_name Human

# Only setter method established
var uniqueName = "John" setget setFunction

func setFunction(param1):
   uniqueName = param1
```

To use only a setter, start with adding a comma `,` followed by the name of the setter
method:

```csharp
extends Node
class_name Human

# Only getter method established
var uniqueName = "John" setget , getFunction

func getFunction():
   return uniqueName
```

### When to use Setter & Getter Methods

Use a setter/getter method when you want to do the following:

- When you need to know when a value has had its value changed

- When you need to perform an action if a variable value has changed

- When you want to protect a variable from having the value changed

# [Fake Protected Variables](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-23)

With the `setget` keyword’s power, you can protect your variables from being used outside of the class your variables are created from.

```csharp
extends Node
class_name Animals

var _protectedVar:String = "Protected Variable" setget protectedSet, protectedGet

func protectedSet(param1):
  print('Can\'t Access Private Variable Setter')

func protectedGet():
  print('Can\'t Access Private Variable Getter')
```

By creating a setter and getter method that neither changes the value
 of the variable nor returns back its value, you will have created a 
variable in which no other class has access to its value.

### Memory Management

Game programming is part coding and part of memory management.

Understanding memory management can help you understand where 
problems are happening with your game. Such issues may include lag or 
random game freezes.

# [Reference Class](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-24https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-24)

In Godot GDScript, all classes that don’t define an inheritance through the `extends` keyword
will inherit from the reference class by default.

```csharp
# Omitting the extends keyword is the same as the following
extends Reference
```

The `Reference` class is the base class for any game object that keeps a reference count.

Reference counting is a memory management technique.

This means that the class will release itself from memory when it is no longer used.

This works because an object will be released from memory when the reference count is `0`.

### Object Class

If you would like to have a game object stay in memory even when it is no longer being used,
you will have to inherit from the `Object` class.

```csharp
extends Object
```

To free a game object which inherits from the object class from memory, you will have
to call the `free` method.

Many of Godot’s built-in Classes inherit from the Object class. This includes the Node class and the Node2D class.

Many problems beginners have when programming with Godot is freeing Nodes from memory.

```csharp
# An example of freeing a Sprite Node from memory
# Sprite Node ultimately inherits from Object class
extends Sprite

class_name MainCharacter

_exit_tree():
    free() # unsafe
```

Another way of deleting from memory:

```csharp
# An example of freeing a Sprite Node from memory
# Sprite Node ultimately inherits from Object class
extends Sprite

class_name MainCharacter

_exit_tree():
    queue_free() # safe
```

# [Cyclic Dependency](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-24-1)

Cyclic Dependencies, also referred to as “Circular Dependencies”, is a
 relation between two or more objects which either directly or 
indirectly depend on each other to function correctly.

The last game object references the first resulting in a closed-loop.

![Cyclic Dependency.png](C:\Users\wrmik\Documents\Godot\Resources\Cyclic%20Dependency.png)

To spell out what is happening:

- `Class_A` depends on `Class_B`
- `Class_B` depends on `Class_C`
- `Class_C` depends on `Class_A`

In this case, the program or application throws an error as it does not know which class to initialize first.

To fix a Cyclic Dependency, simply ensure the dependencies of classes are not in a closed loop.

![Open Loop Dependency.png](C:\Users\wrmik\Documents\Godot\Resources\Open%20Loop%20Dependency.png)

In this case:

- `Class_A` depends on `Class_B`
- `Class_B` depends on `Class_C`
- `Class_C` does not depend on `Class_A`

Therefore the dependencies of the classes are in an open loop.

### Signals

Godot Offers a way to emit messages from one object to another through the use of signals.

To create a signal, you need to create an observer class and a subject class.

A subject class emits a signal to the observer class. In contrast, 
the observer class performs an action once it has received a call/signal
 from the subject class.

In a sense, the subject class is expected to fire a signal; an observer needs to subscribe to a subject.

Both the subject class and the emitter class must be present on the 
scene tree. That means both classes need to be a node on the scene tree.

![Signals.png](C:\Users\wrmik\Documents\Godot\Resources\Signals.png)

To create a Subject class, use the `signal` keyword.

`signal <signal name>`

To send signals to observables, you need to call the `emit_signal` method.

The emitted signal has one mandatory argument and optional argument if you want to pass data to the observables.

`emit_signal(<signal name>, <optional data to pass>)`

To create an observable, you need to create a variable instance of the Node on the
scene tree, followed by calling the signals `connect` method.

The `connect` method takes in 3 mandatory arguments and additional optional arguments
if you want to pass data to the observables.

`connect(<signal name>, <node you want to call function in>, <function to call>)`

Let’s take a look at a complete example:

```csharp
# Subect Class
# Name in Scene: Player
# node Type: Sprite
extends Sprite
signal healthChanged # create the signal called healthChanged

var check: int = 0
var playerHealth: int = 100

func _process(deltaTime):
   if check < 1:
      check = check + 1
      changeHealth(-100)

func changeHealth(value):
   playerHealth = playerHealth + value
   emit_signal("healthChanged", playerHealth) # Emit the signal to observables
```

In this example, we have a Node on the Scene tree called `Player`, and we would like to create a signal that emits every time the players' health has changed.

On top of that, we pass the value of the players' current health to the observables.

In this case, we want to know when the method called `changeHealth(value)` has been called.

The Player Node is considered the subject class.

```csharp
# Oberver Class
# Name in Scene: Health
# node Type: Node2D
extends Node2D

onready var PlayerNode = get_node('Player') 

func _ready():
  PlayerNode.connect("healthChanged", self, "doSomething") # Connect to signal

func doSomething(playerHealth):
  print('We changed value of health to: ', playerHealth)
```

The script above is attached to the scene in a Node called `Health`.

You create an instance to the Player node with `onready var PlayerNode = get_node('Player')`.

Then you connect to its signal with `PlayerNode.connect("healthChanged", self, "doSomething")`.

# [Coroutines and Yield](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-26)

**Coroutines**: A computer component that generalizes 
subroutines for non-preemptive multitasking by allowing execution to be 
suspended and resumed.

Subroutines: a set of instructions designed to perform a frequently used operation
within a program

To understand coroutines, we need to know how sequential processing works.

### Sequential Processing

Sequential processing runs code line by line in sequence, from start to finish in the order it is received in.

In GDScript, your code runs sequentially unless otherwise specified (threads).

Let’s take a look at this example:

```csharp
func _ready():
    addHealth(10)
    print('finished!')

func addHealth(lifePoints):
    print('lifePoints called!')
```

Now let us look at how the code runs sequentially.

![Sequential Code.png](C:\Users\wrmik\Documents\Godot\Resources\Sequential%20Code.png)

Typically, code is run line by line. A function has code inside which needs to run everything first, and only take
a brief moment to pause if a function has been called.

Such is the case where the `_ready()` method will run all the code inside its block unless another
method has been called, in which the block will be pause and move onto the newly called function (`addHealth(lifepoints)`).

### How to use Coroutines

To use coroutines, you will need to use two methods, the `yield` method and the `resume` method.

The `yield` method pauses a function, while the `resume` method will continue the
yielded method.

```csharp
func _ready():
    var pausedFunction = addHealth(10)
    print('finished!')
    pausedFunction.resume() # resume the addHealth call

func addHealth(lifePoints):
    yield() # pause the function
    print('lifePoints called!')
```

![Coroutines.png](C:\Users\wrmik\Documents\Godot\Resources\Coroutines.png)

### Learn More

To learn more about coroutines and yield in the context of GDScript, check out this great resource from [GDScript Dude](https://gdscript.com/solutions/coroutines-and-yield/).

# [Threads](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-27)

Thread is short for thread execution. It is a way for a program to divide itself into two or more simultaneously running tasks.

Threads are a form of concurrent processing, often referred to as 
multi-tasking. They are used to balance the processing power across 
CPU’s and cores.

Concurrency is when the execution of multiple tasks is interleaved. Compared to being executed sequentially one after another.

To create a thread, you will need to instantiate a class from the `Thread` global class.

To start a thread, you will need to use the threads `start` method.

```csharp
var thread = Thread.new()
thread.start(<Object Instance>, <String Method>)
```

# [Static & Dynamic Programming Languages](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-28)

All languages are designed to translate human-readable code into machine instructions.

### Static Language

Type checking occurs at compile time.

A variable doesn’t need to be defined before it is used.

Static Languages: Java, C++

```cpp
// C++ Example
int UniqueName;
uniqueName = 5;
```

### Dynamic Language

Type checking occurs at runtime.

Variables must be defined before they are used.

Dynamic Languages: Javascript, PHP

```php
// PHP Example
$txt = "Hello world!";
```

### Strong Typing

Variables are bound to a data type.

```cpp
// C++ Example
int UniqueName;
uniqueName = "String"; // Throws error, variable can only have integers
```

### Weak Typing

Variables are not bound to a data type.

```csharp
# GDScript Example
var item = 5;
item = "Hello" # Data type can be changed for variabl
```

# [How to Improve Your Programming Skills](https://godottutorials.com/courses/introduction-to-gdscript/godot-tutorials-gdscript-last)

Improving yourself in any skill is dependable on many factors.

I list out a few things you can do as a beginner to improve yourself.

#### Problem Solving

Programming is just problem-solving. If you can do that, then congratulations, you are a programmer!

Problem-solving will be the core of how you will tackle programming challenges, especially in game programming.

To tackle problem-solving effectively, you need to understand two things.

1. Understand the Programming Language
2. Understand the Framework you are using

In this case, GDScript is the programming language, and the Godot application is the framework.

The same can be said for Unity. In Unity, C# is the programming 
language. In contrast, Unity is the framework that will provide you the 
tools for game programming.

#### Programming Patterns

The next step is to understand programming patterns.

Understand the following:

1. Design Patterns
2. Design Principles

The two go hand in hand, and you will benefit lots from understanding them.

#### Math/Physics

Game programming is math.

If you can understand math, you can do game programming.

You don’t have to get into calculus to get into game programming.

It is recommended to have a basic understanding of the following:

- Geometry
- Physics (Speed, Acceleration)
- Basic Trigonometry

#### Algorithms

Algorithms are core to programming.

In many cases, algorithms are a higher level of programming, but it 
is standard that programmers understand some basic algorithms.

At a minimum, understand the algorithm for traversing a 2D array.

### Final Note

I wish you the best on your programming journey.

Thank you so much for letting me be a part of your journey!