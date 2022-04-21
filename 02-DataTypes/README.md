# Data Types

## Overview
Information comes in various forms. 

We can categorise the kinds of data we need to use in our code by classifying them into data types.

A data type is an attribute of data that tells us how a programmer intends to use the data.

Data types define the operations that can be done on the data, the meaning of the data, and the way values of that type can be stored.

We have already seen a few data types in action: `float` and `int`.

We have also used one data type without knowing its name:

![dataType-1](https://imgur.com/otdhpzJ.png)

### ***Strings***
A **String** is declared by encasing any other text in a set of inverted commas or speech marks.

Essentially, a String is a block of text.

There are a number of things to bear in mind when using Strings in Python:

- It is known as a `str`
- `input()` defaults the return value to a String – hence why we cast it
- We can **concatenate** Strings by using `+`:

    ![strings-1](https://imgur.com/ZtojH1M.png)

- Within the print function, we can combine Strings with other data types by using `,`:

    ![strings-2](https://imgur.com/5YYkxem.png)

- We can write Strings over multiple lines by using `\n`:

    ![strings-3](https://imgur.com/V1JSEcY.png)

### ***Integers and Floats***
These are the two main **numeric data type**s in Python.

The difference between **numeric** and **non-numeric** data is that we can use numeric data in calculations, as we’ve already seen.

The key difference between `float` and `int` is that the former uses decimal points, while the latter does not.

### ***Booleans***
A **Boolean** is a data type that is usually treated as non-numeric. 

It can only hold one of two values: `True` or `False`. 

In Python, it is symbolised by the term `bool`.

Booleans are used for logical tests:

- Is something bigger?
- Has something been completed?
- Has a condition been fulfilled?

They are used in tandem with conditional statements.

## Tutorial

Data types of variables are set when the variable is assigned a value:

        Note: The data type of a variable is not fixed. If a different value is assigned to the variable, the data type is updated as well. 

```Python
# Variable                    Data Type
#------------------------------------------
s = "Hello World"             # str
i = 19                        # int
f = 19.4                      # float
b = True                      # bool
```
        Note: Hash symbol(#) in Python is used when writing comments about the code. Python ignores any text after a # in a line.

We can also set specific data types to variables like so:

```Python
s = str("Hello World")
i = int(19)
f = float(19.4)
b = bool(True)
```

## Exercises

### Exercise 1: Playing around with Strings

1. Create a file named Strings.py for this task.
2. Write some code that uses some of the String-concepts we have already covered.

### Exercise 2: Playing around with numeric data types

1. Create a file named Numeric.py for this task.

    ![code-snippet](https://imgur.com/uACiMPo.png)

2. Using the code snippet above, print out the results of casting these numbers.
3. What do you notice about them?

### Exercise 3: Rounding

1. Create a file named Rounding.py for this task.
2. Replicate the code setup below:

    ![code-snippet-2](https://imgur.com/Z5vFHm3.png)

3. Before running this code, write down what you think the output will be.

### Exercise 4: Working with Booleans

1. Create a file named Booleans.py for this task.
2. Replicate the code below in your file:

    ![code-snippet-3](https://imgur.com/UYsLeUE.png)

         We can see here that we have a condition. If fulfilled, then number1bigger would be set to be True else if the condition is not met, then number1bigger would be set to be False.

3. What do you think the code is doing in the middle section highlighted in red?
