
- [1. Introduction to the high-level language python](#1-introduction-to-the-high-level-language-python)
- [2. Data type](#2-data-type)
- [3. Print data to the screen](#3-print-data-to-the-screen)
  - [3.1. print( )](#31-print-)
  - [3.2. format (parameter )](#32-format-parameter-)
- [4. Get data from user](#4-get-data-from-user)
- [5. Comment](#5-comment)
- [6. Operators in Python](#6-operators-in-python)
  - [6.1. Aithmetic Operators](#61-aithmetic-operators)
  - [6.2. Comparison Operators](#62-comparison-operators)
  - [6.3. Assignment Operators](#63-assignment-operators)
  - [6.4. Logical Operators](#64-logical-operators)
- [7. Condition statement in Python](#7-condition-statement-in-python)
  - [7.1. Syntax condition statement](#71-syntax-condition-statement)
  - [7.2. Ternary Operator in Python](#72-ternary-operator-in-python)
  - [7.3. Elif Statement](#73-elif-statement)
  - [7.4. Nested If Statements](#74-nested-if-statements)
- [8. Python Loops](#8-python-loops)
  - [8.1. For Loops](#81-for-loops)
    - [8.1.1. Syntax For Loop](#811-syntax-for-loop)
    - [8.1.2. Iterating Over a List](#812-iterating-over-a-list)
    - [8.1.3. Nested For Loop](#813-nested-for-loop)
  - [8.2. While loop](#82-while-loop)
    - [8.2.1. Syntax While Loop](#821-syntax-while-loop)
    - [8.2.2. Nested While Loop](#822-nested-while-loop)
- [9. Break and Continue Statements in Python](#9-break-and-continue-statements-in-python)
  - [9.1. Break](#91-break)
  - [9.2. Continue](#92-continue)
- [10. Function](#10-function)
- [11. Class](#11-class)
- [12. GUI](#12-gui)


## 1. Introduction to the high-level language python
https://en.wikipedia.org/wiki/Python_(programming_language)
## 2. Data type
In python there are the following data types: integer (int), float(float), boolean(bool), string(str)
>Note: You do not need to specify the data type for a variable when you declare it. Instead, the data type is determined based on the value you assign to that variable.

Example:
```Python
x = 3 # x bring style int
y = 0.45 # y bring style float
check = True # check bring style boolean
t = "This is a string" # t bring style string
```
## 3. Print data to the screen
We often use `print()` or `format()` to print data to the screen in Python
### 3.1. print( )
Example: 
```Python
#To print a string, we need to add double quotes for the paragraph to print, for number 
print("ABC123") # print a string ABC123
text = "To day you so beautiful"
print(text) # print a string into text to the screen
print(27) # print number 27 
age = 18
print(age) # print a number into age variable, data type is int 
# print("age") != print(age) 
print(str(age)) # Now age data type is string
print("I am " + str(age) + " years old") # can't not connect string with integer
# We use syntax `data type()` to  type conversion.
# We use `+` to connect two string 
```
### 3.2. format (parameter )
We use `{}` and `parameter` in format to print
```Python
name = "Bob"
age = 25
print("My name is {} and I am {} years old.".format(name, age))#Positional references to parameters in the format function
```
## 4. Get data from user
We use `input()` to get data from user
Example: 
```python
age = input("Enter age")
```

## 5. Comment
We use `#` to comment 
Example: 
```Python
# this is comment  
```
## 6. Operators in Python

Python supports various types of operators, including arithmetic, comparison, assignment, logical, and more. Below is an overview of these operators.

### 6.1. Aithmetic Operators

Arithmetic operators are used to perform basic mathematical operations.

| Operator | Description         | Example  |
| -------- | ------------------- | -------- |
| `+`      | Addition            | `a + b`  |
| `-`      | Subtraction         | `a - b`  |
| `*`      | Multiplication      | `a * b`  |
| `/`      | Division (float)    | `a / b`  |
| `//`     | Division (floor)    | `a // b` |
| `%`      | Modulus (remainder) | `a % b`  |
| `**`     | Exponentiation      | `a ** b` |

### 6.2. Comparison Operators

Comparison operators are used to compare two values.

| Operator | Description              | Example  |
| -------- | ------------------------ | -------- |
| `==`     | Equal to                 | `a == b` |
| `!=`     | Not equal to             | `a != b` |
| `>`      | Greater than             | `a > b`  |
| `<`      | Less than                | `a < b`  |
| `>=`     | Greater than or equal to | `a >= b` |
| `<=`     | Less than or equal to    | `a <= b` |

### 6.3. Assignment Operators

Assignment operators are used to assign values to variables.

| Operator | Description             | Example   |
| -------- | ----------------------- | --------- |
| `=`      | Assign                  | `a = 5`   |
| `+=`     | Add and assign          | `a += 2`  |
| `-=`     | Subtract and assign     | `a -= 2`  |
| `*=`     | Multiply and assign     | `a *= 2`  |
| `/=`     | Divide and assign       | `a /= 2`  |
| `//=`    | Floor divide and assign | `a //= 2` |
| `%=`     | Modulus and assign      | `a %= 2`  |
| `**=`    | Exponentiate and assign | `a **= 2` |

### 6.4. Logical Operators

Logical operators are used to combine conditional statements.

| Operator | Description                                    | Example            |
| -------- | ---------------------------------------------- | ------------------ |
| `and`    | Returns True if both statements are true       | `a > 5 and b < 10` |
| `or`     | Returns True if at least one statement is true | `a > 5 or b < 10`  |
| `not`    | Returns True if the statement is false         | `not(a > 5)`       |

## 7. Condition statement in Python

The `if-else` statement is a fundamental control flow structure in Python that allows you to execute specific code based on certain conditions. It is essential for making decisions in your programs.

### 7.1. Syntax condition statement

```python
if condition:
    # Code to execute if condition is True
else:
    # Code to execute if condition is False
```
Example: 
```python 
x = 3
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```
### 7.2. Ternary Operator in Python

The ternary operator is a shorthand way to write conditional expressions. Its syntax in Python is as follows:

```python
<true_value> if <condition> else <false_value>
```
Example:
```python
a = 5
b = 10
max_value = a if a > b else b
print(max_value)  # Output: 10
```

### 7.3. Elif Statement
The elif (short for "else if") statement allows you to check multiple conditions. If the first if condition is False, it checks the elif condition.
Example:
```python 
x = 5
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
```
### 7.4. Nested If Statements
You can nest if statements within other if statements to check multiple conditions.
Example:
```python
x = 10
if x > 5:
    print("x is greater than 5")
    if x > 8:
        print("x is also greater than 8")
    else:
        print("x is not greater than 8")
else:
    print("x is not greater than 5")
```
## 8. Python Loops
Loops are fundamental in programming, allowing you to execute a block of code multiple times. In Python, the primary types of loops are `for` loops and `while` loops.

### 8.1. For Loops

The `for` loop in Python is used to iterate over a sequence (like a list, tuple, or string) or to iterate over a range of numbers.

#### 8.1.1. Syntax For Loop
```python
for i in range(number_star,number_end; number_jump)
    # Code
# OR 
for i in list
    #code
```


Example:
```python
for i in range(5):
    print(i) #loop through i 5 times and increment i by 1
for i in range(0,5,1) # similar for loop C++: for(int i = 0; i<3; i++)
    print(i)
```
>Output: 
0
1
2
3
4

#### 8.1.2. Iterating Over a List
You can iterate through the elements of a list using a for loop.
Example:
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:#loop fruit until the list is exhausted
    print(fruit)
```
>Output: 
apple
banana
cherry

#### 8.1.3. Nested For Loop
Example:
```python 
for i in range(3):
    for j in range(2):
        print("i: {}, j: {}".format(i,j))
```
>Output:
i: 0, j: 0
i: 0, j: 1
i: 1, j: 0
i: 1, j: 1
i: 2, j: 0
i: 2, j: 1



### 8.2. While loop
A while loop continues to execute as long as its condition is True.

#### 8.2.1. Syntax While Loop
```python
while condition:
    # Code to execute if condition is True
```


#### 8.2.2. Nested While Loop
Example:
```python 
i = 0
while i < 3:
    j = 0
    while j < 2:
        print("i: {}, j: {}".format(i,j))
        j += 1
    i += 1
```
>Output:
i: 0, j: 0
i: 0, j: 1
i: 1, j: 0
i: 1, j: 1
i: 2, j: 0
i: 2, j: 1

## 9. Break and Continue Statements in Python
In Python, `break` and `continue` are control flow statements that alter the flow of loops. They help manage loop execution based on certain conditions.

### 9.1. Break
You can use the break statement to exit a loop prematurely.
Example:
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```
>Output:
0
1
2
3
4
### 9.2. Continue 
The continue statement is used to skip the current iteration of a loop and proceed to the next iteration.
Example:
```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```
>Output
1
3
5
7
9
## 10. Function

## 11. Class

## 12. GUI
