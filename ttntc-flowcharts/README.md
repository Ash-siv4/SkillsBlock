# Flowcharts

## Overview

A good way of breaking down a problem into clear steps is to use a **flowchart**.

Flowcharts are a graphical representation of a set of instructions.

They are often used in programming to plan out the steps required for the application to function as required.

### ***Symbols***

The following standard symbols are used to construct a flowchart and each symbol represents a different type of instruction.

|   Symbol   |   Meaning    |   Description    |
|   ---     |   ---     |   ---     |
|   ![oval](https://i.gyazo.com/290789f6e0defec097685662d4a62e6b.png)              |  **`START / END`**     |   Oval shapes are used to represent the start and end points of the flowchart |
|   ![arrow](https://imgur.com/a8MLWGe.png)             |  **`FLOW LINES`**      |   Arrows *(also known as flow lines)* are used to connect the symbols in a flowchart and indicate the direction of flow |
|   ![parallelogram](https://i.gyazo.com/d10135f1f6908810de49a11b44b0e49b.png)     |  **`INPUT / OUTPUT`**  |   Parallelograms are used to illustrate inputs and outputs, which are usually user actions |
|   ![rectangle](https://i.gyazo.com/77424a0f518215a7371e5a38067ffb27.png)         |  **`PROCESS`**         |   Rectangles symbolise processes such as calculations like arithmetic operations |
|   ![diamond](https://i.gyazo.com/a17d61c920001e05387d25ed99b55946.png)           |  **`DECISION`**        |   Diamond shapes indicate a point of decision  |

## Tutorial

Given the requirement, to write a piece of code which checks to see if an inputted number is even:

1. First create a flowchart to have a step-by-step approach to the problem.
2. Use the flowchart as a guide to writing the code to solve the problem. 

### Solving the problem by creating a flowchart

Breaking down the problem into smaller steps:

1. Start
2. Process - Initialise a value for comparison
3. User input - Ask the user to enter a number,
4. Decision - Compare the input against the stored variable
5. Output - Print odd or even depending on the decision
6. End

Here is the flowchart designed based on the previously stated steps:

![flowchartTutorial](https://i.gyazo.com/149cc4db9914ee4eaabc6172209a2f7e.png)

### Writing the code

Generating the code based on the flowchart:

```Python
zero = 0
num = int(input("Please enter a number: "))
if num % 2 == zero:
  print(num,"is even")
else:
  print(num,"is odd")
```

Each line of code is a step in the flowchart.

## Exercises

### Exercise 1: Reverse engineering a flowchart

1. Given the code below, create a flowchart to illustrate it.

```Python
password = "Hello World"
user = input("Please enter your password: ")
if password == user:
  print("Password is correct")
else:
  print("ERROR: Try again")
```

### Exercise 2: Print the largest number

1. Take a look at the following flowchart and write the `python` code for it.

    ![flowchartEx](https://i.gyazo.com/27613a06bbb2e0170d271c0446370658.png)

2. Test your code with the following values:

    - a = 5, b = 10, c = 12 -> **prints c**
    - a = 19, b = 23, c = 4 -> **prints b**
    - a = 228, b = 67, c = 93 -> **prints a**
