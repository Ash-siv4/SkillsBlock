# Introduction

## Overview

In this module, we will look at why we need computers as well as give an introduction to variables.

### Why do we need computers?

Most of us use computers as part of our everyday lives, either for work or for personal use, but why do we use computers?

Most people think that computers will solve problems for us, however, computers do not solve the problems, we do.

In Teach The Nation To Code, you will hear the phrase **a computer is a stupid machine** many times.
This is because computers will only ever do exactly what they are told to do, they cannot do any more.

So then, why do we need computers?
The answer is for two reasons: speed and accuracy.
These two reasons are what make computers incredibly useful in helping us solve problems.

#### Speed

If you were asked to calculate 
> 378 x 183 = ?

It would take a while to work out, for even the quickest Mathematician this might take 10-20 seconds, a computer will do it in less than 1.

#### Accuracy

If a group of 100 people were asked to calculate
> 378 x 182 = ?

Even with as much time as you need, the chances are we would still get some different answers, whereas 100 computers would all give the same answer.

### Why do we need variables?

Let's say we have some complicated information which we need to use over and over.
For example, a long number such as Mathematical Pi

`3.14159265358979323846`

Instead of writing this out multiple times within a program, we can instead store it in an easily accessible location. This is where variables come in.

A variable is a callable keyword which references a place in the memory where the information is stored.
We do not know where in the memory this information is stored, and we don't need to, since the address is attached to the variable (invisible to us).

```python
pi = 3.14159265358979323846
print(pi)
```

In the second line, we ask Python to print to the terminal the value of the variable `pi`, which is easier than writing out the whole thing again.
The variable points to the location in our computer's memory where the value is stored, and Python can then use it.

### Working with variables

#### Assignment

We store a value in a variable using the **assignment operator** (`=`).

This stores the **value** on the right hand side, in the location referenced by **variable name** on the left hand side.

```python
pi = 3.14159265358979323846
```

#### Reassignment

So far, we've not really seen why a variable is called a variable.
However, we can **reassign** the value of a variable.

Let's say that we have a variable but we want to change its value, we can do that, again using the **assignment operator**.

```python
a = 10
b = 20
a = 40
print(a)
```

This would print to our terminal the value `40` since the variable `a` has been reassigned from 10 to 40.

#### Expressions

Python is able to do Mathematical calculation using variables.
To do this we use the **mathematical operators**.

| Operator | Name |
| ---| --- |
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |

These are the standard operators but there are many more.

Let's see some examples:

```python
a = 10
b = 20
c = 50 + 50
d = a + b
```

On the third line, Python will do the calculation `50 + 50` and then store the result (100) in `c`.

On the fourth line, Python will find the value of `a` (10), find the value of `b` (20), add those values together (30) and then store the result in `d`.

#### Execution

It is important to understand the order that Python runs commands.

Like most programming languages, Python starts at the top of the file and works it's way to the bottom.

```python
a = 10
b = 20
c = a + b
a = 40
print(c)
```

What would the final line print to our terminal?

Well, let's go through it as Python would.
1. First, we assign the value of 10 to the variable `a`.
2. Next, we assign the value of 20 to the variable `b`.
3. Then, we find the value of `a` (10), the value of `b` (20) and add them together (30) and store it in the variable `c`.
4. Then, we reassign the value of `a` to be `40`.
5. Finally, we find the value of `c` (30) and print it to the terminal.

So, the final line prints `30` to the terminal.

#### Specificity

The programs we've written so far are good, but they're not very reusable.

Let's make a very simple program for calculating the combined score for all your science exams.
We will store the value of our biology, chemistry and physics marks in variables, then add them all together and store the total in a variable.

```python
a = 60
b = 70
c = 80
d = a + b + c
```

Although this will function exactly as we want, if we look back at it in a few weeks time, we will have no idea what `a`, `b`, `c` & `d` were for.

We should always give our variables **meaningful names**!

Let's rewrite the previous program.

```python
biology = 60
chemistry = 70
physics = 80
total = biology + chemistry + physics
```

This is much easier for us to understand what the program is doing.

### Inputs

So far, we have assumed that the person writing the program is the one who will be using it; this is not always the case.

Let's look at the exam calculator from before.

If someone, who is not the person who wrote the program, wanted to use it, they wouldn't be able to put their own values in.
This is because we have **hard-coded** the values in the program.

To make the program usable by anyone, we will use the **input function** to allow the user to enter their own marks.

```python
biology = input()
chemistry = input()
physics = input()
total = biology + chemistry + physics
```

Every time Python gets to the input function, it will wait for the user to input a value.
If there is any text inside the brackets, it will print that to the terminal and then wait for the user to input a value.

So our final program for this module should be:

```python
biology = input("Please enter your Biology marks: ")
chemistry = input("Please enter your Chemistry marks: ")
physics = input("Please enter your Physics marks: ")
total = biology + chemistry + physics
```

## Tutorial

In this tutorial, we will create a program which will take in English, Maths, and Science scores and then calculates their average score.

1. First, we need to store the scores inside variables to use later on.
```python
english = 50
maths = 60
science = 70
```
2. Now, we need to calculate the average. 
To do this, we need the **total marks** which we can store in a variable, and then we will divide the total by 3 in order to get the average.
We will store the final result in another variable.
```python
total = english + maths + science
average = total / 3
```
3. Lastly, we will print the average to the terminal with a nice message.
```python
print("Your average score is :")
print(average)
```

## Exercises

Try to improve the program we created to allow the user to enter their own scores.

<details><summary>Hint</summary>

You can use the `+` operator on words.
`print("hello"+"world")` will give us `helloworld`.

Take a look at the **Data Types** module for more information.

</details>
