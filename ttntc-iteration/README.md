# Iteration

## Overview

Iteration is simply repeating processes over and over again.
In this module, we will look at how to create iterating processes in Python, specifically **while loops** and **for loops**.

### While Loops

A `while` loop checks if a condition is true, then completes a set of instructions, just like an `if` statement.
The difference is that, if the condition is `True` after the set of instructions have been completed, Python will go back and check the condition again.
If the condition is still true, Python will then execute the set of instructions again and it will keep doing so until the condition becomes `False`.
As soon as the condition is false, Python is finished with the loop and will carry on executing the rest of the file below.

We can liken this kind of loop to counting in our heads.
For example, let's say someone asks you to say the letter "h" 10 times. You will keep count in your head and each time you say the letter "h", you will add one to that count.

Let's see this in Python:
```python
count = 0
while count < 10:
    print("h")
    count = count + 1
```

> Note: The condition doesn't have to be a count, any conditional statement would work there.

### For Loops

A `for` loop is used to repeat a set of instructions a specific number of times.

For loops are often used with the `range` function.

```python
for i in range(11):
    print(i)
```

Here, `i` is known as the iterator and for each iteration, it will take a different value.

#### Range

The range function takes up to 3 arguments `range(start,stop,step)`.
- `start` - the number to start at, defaults to 0 if not specified (it **will** include this number).
- `stop` - the number to stop before (it will **not** include this number).
- `step` - the number to increment each time, defaults to 1 if not specified.

eg:
- `range(101)` will give `0, 1, 2, 3,..., 100`
- `range(1,5)` will give `1, 2, 3, 4`
- `range(1,10,2)` will give `1, 3, 5, 7, 9`

### Break

If we want to `finish` a loop before the set endpoint, we can use the keyword `break`.

```python
for i in range(101):
    print(i)
    if i == 20:
        break
```

This will print out the numbers 0 to 20 and then break out of the loop.

### Continue

If we want to skip an iteration of the loop, we can use the keyword `continue`.

```python
for i in range(101):
    if i == 20:
        continue
    print(i)
```

This will print out all the numbers 0 to 100, **except** for 20, which it will skip.

## Tutorial

In this tutorial, we will look at two different ways to print all the **even** numbers between 1 and 10 inclusive.

> A number is **even** if it is divisible by 2 with no remainder.

To find the remainder in Python, we use the `%` operator.
e.g. `4 % 2 = 0` and `5 % 2 = 1`.

1. We will first use a `while` loop.
```python
number = 0
while number <= 10:
    number = number + 1
    remainder = number % 2
    if remainder == 1:
        continue
    print(number)
```

2. We will now use a `for` loop.
```python
for number in range(1,11):
    remainder = number % 2
    if remainder == 1:
        continue
    print(number)
```

## Exercises

### Exercise 1: Looping through
1. Create three different `loop.py` files for this task (name them accordingly).
2. Set up each file according to the below code:

```python
#File 1
for i in range(101):
    print(i)

#File 2
for i in range(5,10):
    print(i)
    
#File 3
for i in range(10,21,2):
    print(i)
```

3. Before you run any of these files, try to work out what the output of each will be.

### Exercise 2: Zero
1. Create a file named `Zero.py` for this task.
2. Replicate the code below.
What do you expect it to do if it is run?
```python
count = 0
while count < 3:
    print(count)
```
3. Rewrite the code so that it includes 3.

### Exercise 3: Odd/Even
1. Create a file named `OddEven.py` for this task.
2. Replicate the following code within your file:
```python
count = 0
while count < 9:
    count = count + 3
    if SOMETHING:
        print(count, "is even")
    else:
        print(count, "is odd")
```
3. Replace `SOMETHING` with an expression to check if the value stored in `count` is even.
You can use the tutorial to help you.

### Exercise 4: TimesTable
1. Create a file named `TimesTables.py` for this task.
2. Write a program which writes the
times tables up to 10.
3. The first output should read `1*1=1`.
The last output should read `10*10=100`.

<details><summary>Hint</summary>

You can use this as a template if you're stuck.
```python
number1 = 
while number1 <=  :
    number1 = 

    while  <= 9:

        print(number1, "x",   , "=", number1 *   )
```
There are spaces left blank for you to fill in.
