# Exercises

## Overview

In this module, you will look at how to approach two different types of problems in order to create solutions for them in Python.

## Tutorial

### Working from Flowcharts

For these types of problems, you will be given a **flowchart** which you will need to convert into Python syntax.
This type of exercise will require you to think logically about what the flowchart is doing before attempting to translate it.

#### Recap

In flowcharts:
- Oval - represents the `Start` and `End` of our program.
- Rectangle - represents processes done in single lines of code.
- Parallelogram - represents an input or an output.
- Diamond - represents a condition.

#### Example 1

Take a look at the following flowchart:

![Image from Gyazo](https://i.gyazo.com/d5cf2e3f8aa28fe77e094a1d2b960fdb.png)

We can see that the program needs to take an input, then, depending on the value of the input, print an output, then end.

Try and work this out on your own before looking at the solution below.

<details><summary>Answer</summary>

```python
num = int(input('Please enter a number: '))
if num % 2 == 0:
    print(num, "is even")
else:
    print(num, "is odd")
```

</details>

### Working from Solutions

For these types of problems, you will be given an **output**, from which you will need to write the code to produce that output.
This type of exercise will require you to think about what has been outputted, a logical way to get that output, and then create the Python code to do it.

Creating your own **flowchart** for the logic may be useful here.

#### Example 2

Take a look at the following output:

```
1
12
123
1234
12345
```

We can see that the program is counting all the numbers from `1` to `5` in a sequence.

> You may wish to draw out your own flowchart for this.

We can see that we are going to need at least two variables:

1. A variable to act as a counter which will stop when we get to 5.
2. A variable to be printed each time we loop.

Try and work this out on your own before looking at the solution below.

<details><summary>Answer</summary>

```python
counter = 1
output = ""

while counter <=5:
    output = output + str(counter)
    print(output)
    counter = counter + 1
```

</details>

## Exercises

Write the Python solutions to the following exercises, these will be in one of the two forms discussed in the module.


### Exercise 1

![Image from Gyazo](https://i.gyazo.com/0d64386d132f0be6198baa807a962c15.png)

### Exercise 2

![Image from Gyazo](https://i.gyazo.com/05d67aa3b77837fc32bd2caf6253c0d3.png)

### Exercise 3

![Image from Gyazo](https://i.gyazo.com/adcf5d75a2a2632c39544b5033e9db06.png)

### Exercise 4

![Image from Gyazo](https://i.gyazo.com/49ec39fb9f501ce8747d131795cc3835.png)

### Exercise 5

![Image from Gyazo](https://i.gyazo.com/27613a06bbb2e0170d271c0446370658.png)

### Exercise 6

![Image from Gyazo](https://i.gyazo.com/678c1411b1f96c4709b8882c49fa0656.png)

### Exercise 7

![Image from Gyazo](https://i.gyazo.com/d7b4df0eb4bffc009c3ae1544af63dba.png)

### Exercise 8

![Image from Gyazo](https://i.gyazo.com/154b8c7f16939fe5312507a57378ebe1.png)

### Exercise 9

![Image from Gyazo](https://i.gyazo.com/1f09447bbe206e7353319f6639e4c333.png)

### Exercise 10

```
1
22
333
4444
55555
666666
7777777
88888888
999999999
10101010101010101010
```

### Exercise 11

```
1.
1,2.
1,2,3.
1,2,3,4.
1,2,3,4,5.
1,2,3,4,5,6.
1,2,3,4,5,6,7.
1,2,3,4,5,6,7,8.
1,2,3,4,5,6,7,8,9.
1,2,3,4,5,6,7,8,9,10.
```

### Exercise 12

```
2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
```

### Exercise 13

```
Enter a number: 5
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

### Exercise 14

```
Enter the first number: 7
Enter the second number: 17
Table of 7
7 x 1 = 7
7 x 2 = 14
...
...
7 x 10 = 70
Table of 8
8 x 1 = 8
...
...
Table of 17
17 x 1 = 17
...
...
17 x 10 = 170
```
