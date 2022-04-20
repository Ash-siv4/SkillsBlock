# Conditionals

## Overview

Often a computer program must make choices on which way to proceed based on certain conditions.

For example, if the temperature is above 30°C then turn on the AC but if it is below then turn on the heater.

Conditional statements such as `if`, `else if` and `else` are used in programming to process conditions.

### ***Control Flow***

Before we look further into **conditionals**, it is important to consider the way in which code executes.

Earlier, we touched on how Python, like every other major programming language, executes from top to bottom. Essentially once a line of code has completed, the compiler will always move down the program by one line.

**Control flow** is simply the order that lines of code are executed in. By using statements which manipulate the flow of a program, the programmer can determine which section of code is run in a program at any time.

It is important to master this art.

It is critical to understand, in any program, which blocks of code are going to execute, and when. This is important not only for writing your own programs, but for reading and understanding code that you haven’t written.

### ***Conditions***

As seen in *Exercise 4: Working with Booleans* in the *Data Types module*, we can write some code which only runs if a condition is true:

![codeSnippet](https://imgur.com/I4KJ60Q.png)

For this set of statements, we know that **number1bigger** will only ever be **True** if **number1** is bigger than **number2**. We define this by using `>` in this case.

### ***Operators***

There are several other operators which can be used within conditional statements, some of which you may recognise from mathematics:

|   Operator    |   Function    |
|   --- |   --- |
|   **`>`**   |   Greater than    |
|   **`<`**   |   Less than   |
|   **`==`**  |   Equal to    |
|   **`!=`**  |   Not equal to    |
|   **`>=`**  |   Greater than or equal to    |
|   **`<=`**  |   Less than or equal to   |

To check if a condition is True, we can use these operators alongside conditional statements.

### ***if:***

The most well-used conditional statement is the **if-statement**. If a condition evaluates to being True, then any code encased within the if-statement is run.

In Python, it looks like this:

![ifSnippet-1](https://imgur.com/O5eqJNU.png)

If, for whatever reason, we assigned a variable called **name** to something that was not ‘Bill’, then the print statement would never run - the compiler would simply skip over that line of code.

![ifSnippet-2](https://imgur.com/lNl0VGR.png)

As you can see, the code which depends on the if-statement is indented. The reason for this is extremely important:

![ifSnippet-3](https://imgur.com/2RxArnu.png)

An indentation is **`4 spaces`** which is also the equivalent of **`1 tab`**.

By laying out code in this way, both the programmer and the compiler can clearly see which blocks of code execute in which situations.

### ***else:***

**Else** is a catch-all conditional statement. It is used to check any cases which an if-statement does not check for.

For instance, let’s look at the following code:

![elseSnippet](https://imgur.com/wBkY8DV.png)

In this code, we ask the user to enter the number 23 – and, in **any** case where the number 23 is not entered, the else-statement will activate and print **False** to the screen.

### ***elif:***

We don’t always need our programs to check if every condition evaluates to True. In a lot of cases, only one condition can be True.

This issue can be solved by using an **else-if-statement**. The else-if-statement is defined in Python as `elif`.

By using an elif-statement, you can make your code more efficient.

## Tutorial

Writing an **if-statement** in Python:

```Python
speed = 23
if speed > 70:
  print("over speed limit")
```

Building on the **if-statement** with an **elif-statement**:

```Python
speed = 23
if speed > 70:
  print("over speed limit")
elif speed == 70:
  print("right speed")
```

Combining the **if**, **elif** and **else** statements:

```Python
speed = 23
if speed > 70:
  print("over speed limit")
elif speed == 70:
  print("right speed")
else:
  print("under speed limit")
```

## Exercises

### Exercise 1: Practicing conditionals

1. Create a file named Conditionals.py for this task.
2. Write a program which asks for an input of a mark, then checks to see if the mark is greater than 65. If so, print out **Pass**. If not, print **Fail**.
3. There are multiple ways of achieving this – but for now, do not use the else statement which you might have noticed we used earlier.

### Exercise 2: if/else

1. Use the file from *Exercise 1: Practicing conditionals* for this task.
2. Update your program to use the **else**-statement to solve the problem.

### Exercise 3: if/elif/else

1. Use the file from *Exercise 1: Practicing conditionals* for this task.
2. Update your program to account for multiple grade boundaries – e.g. a **Merit**, a **Distinction**, a **Pass** and a **Fail** grade.

### Exercise 4: Indentation

1. Create a file called TemperatureGauge.py for this task.
2. Replicate the following code in your file:

    ![exerciseCode-1](https://imgur.com/kV3I417.png)

3. What will happen if we set **temperature** to be 40? 60? 20?
4. What problems are we seeing occur in the code? How can we fix it?

### Exercise 5: Many ifs

1. Use the file from *Exercise 4: Indentation* for this task.
2. Replicate the following code in your file:

    ![exerciseCode-2](https://imgur.com/Zfu2L2I.png)

3. What will happen if we set temperature to 20? 40? -10?

### Exercise 6: And an else

1. Use the file from *Exercise 4: Indentation* for this task.
2. Edit the final if-statement to be an else-statement.
3. What is this implementation doing that makes it different from the several if-statements we used in *Exercise 5: Many ifs*?

### Exercise 7: Improved if/elif/else

1. Use the file from *Exercise 4: Indentation* for this task.
2. Edit the code to use a set of if-, elif-, and else-statements.
3. Why is this implementation better than using the several if-statements written in *Exercise 5: Many ifs*? Think about how each block of your code links together.
4. Why is this implementation better than the if and if-else statements used in *Exercise 6: And an else*?
