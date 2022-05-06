# Farm Project - Python

## Introduction 
The purpose of this document is to outline the python project specification.

This project will involve all the concepts covered in the python beginner session you attended; more specifically, this will involve: 
- Data Types
- Flowcharts
- Conditionals 
- Iteration

## Objective
The overall objective of the project is the following: 

- To create an application in Python and apply all the taught concepts to meet the requirements mentioned in the Scope.

You may use flowcharts to plan the approach you will take to complete this project. 

### Specification
A farmer has approached you with the following dilemma.

The farmer has a farm, which only has `2` types of animals, **chickens** and **cows**. 
The farmer does not know how many of each animal there are, but the farmer was able to count the number of heads and legs there were in total.

The farmer tells you the following:
- Each **chicken** produces `2 eggs per day`, each **cow** produces `4 litres of milk per day`.
- Each **chicken** eats `1/4 bag of corn per day`, and `a bag of corn costs £1.50 each`.
- The farmer `sells each egg for 60p`, and `each litre of milk for 50p`.
- **Tax** on income `less than £12,500 is 0%`, tax on income `£12,500 - £39,999 is 20%`, tax on income `£40,000 or more is 40%`.

At the **`end of the year`**, the farmer goes to market with all the products and wants an invoice with all the details about the animals, products, sales, income, expenses, and profit.

Using only information about the number of heads and legs along with what the farmer has told you above, create an application for the farmer which lists the following:
- Number of chickens on the farm
- Number of cows on the farm
- Number of eggs produced by the chickens
- Volume of milk produced by the cows
- Income from egg sales per day
- Income from milk sales per day
- Total income *before* tax
- Tax amount
- Total income *after* tax
- Total expenses
- Overall profit for the year

## Scope

The minimum requirements set for the project are below.

### Requirements/Output
Print out the farmers' receipt, it should be in the following format:
```
ANIMALS:
chickens = NumberOfChickens
cows = NumberOfCows
------------------------------------
PRODUCTS:
eggs = NumberOfEggs
milk = VolumeOfMilk (litres)
------------------------------------
SALES:
eggIncome = TotalIncomeFromEggs
milkIncome = TotalIncomeFromMilk
------------------------------------
INCOME:
GrossIncome = TotalIncome
Tax = Tax (BasedOnGrossIncome)
NetIncome = CalculatedNetIncome
------------------------------------
EXPENSES:
Corn = TotalSpentOnCornForYear
------------------------------------
PROFIT: FarmersProfit
```

**Test your code with the following heads and legs:**
1. heads: 20, legs: 44

    **Output values:**
    ```
    chickens = 18
    cows = 2
    eggs = 36
    milk = 8 (litres)
    eggIncome = 21.599999999999998
    milkIncome = 4.0
    GrossIncome = 9344.0
    Tax = 0
    NetIncome = 9344.0
    Corn = 2463.75
    PROFIT: 6880.25
    ```
2. heads: 30, legs: 76

    **Output values:**
    ```
    chickens = 22
    cows = 8
    eggs = 44
    milk = 32 (litres)
    eggIncome = 26.4
    milkIncome = 16.0
    GrossIncome = 15476.0
    Tax = 3095.2000000000003
    NetIncome = 12380.8
    Corn = 3011.25
    PROFIT: 9369.55
    ```
3. heads: 124, legs: 272

    **Output values:**
    ```
    chickens = 112
    cows = 12
    eggs = 224
    milk = 48 (litres)
    eggIncome = 134.4
    milkIncome = 24.0
    GrossIncome = 57816.0
    Tax = 23126.4
    NetIncome = 34689.6
    Corn = 15330.0
    PROFIT: 19359.6
    ```

## Constraints
The application needs to be developed in Python.

If you do not have Python installed, you can use an online IDE such as the one used in the Saturday session.

Links to IDE's you can use are here:
- https://repl.it/languages/Python3
- https://www.online-ide.com/online_python_ide
- https://www.programiz.com/python-programming/online-compiler/

## Deliverable 
The final deliverable for this project is the completed application and any flowcharts made during the planning stage.