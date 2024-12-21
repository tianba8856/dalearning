---
category: Python Basics
share: "true"
aliases: 
---

Operators in Python are special symbols that perform specific operations on one, two or more operands (values) and produce a result. Operators can be classified into different categories such as arithmetic, comparison, logical, bitwise, assignment and identity operators, each with a specific purpose.
- Arithmetic operators
- Comparison (Relational) operators
- Logical operators
- Boolean operators
- Assignment operators
- Bitwise operators
- Membership operators
- Identity operators

### Arithmetic Operators

Arithmetic Operators are the basic mathematical operators in Python used to perform arithmetic operations such as addition, subtraction, multiplication, division, and others. These operators are represented by symbols such as `+, -,*, /, %, and **`. They are used to perform mathematical operations on numbers and produce a single output value. For example, addition (+) operator is used to add two values, subtraction (-) operator is used to subtract two values, and so on. With these operators, you can perform various mathematical calculations in Python, making it an ideal choice for numerical computing and data analysis. Additionally, Python provides support for complex numbers, which can be manipulated using arithmetic operators, making it a powerful tool for advanced mathematical and scientific calculations.

| Operator       | Symbol | Description                                                         |
| -------------- | ------ | ------------------------------------------------------------------- |
| Addition       | +      | Adds two values                                                     |
| Subtraction    | -      | Subtracts one value from another                                    |
| Multiplication | `*`    | Multiplies two values                                               |
| Division       | /      | Divides one value by another (returns a float)                      |
| Floor Division | //     | Divides one value by another and rounds down to the nearest integer |
| Modulus        | %      | Returns the remainder of a division operation                       |
| Exponent       | `**`   | Raises a value to a power                                           |

```python
a = 5
b = 2
print(a + b) # 7
print(a - b) # 3
print(a * b) # 10
print(a / b) # 2.5
print(a // b) # 2
print(a % b) # 1
print(a ** b) # 25

# Addition
x = 3 + 4
print(x) # Output: 7

# Subtraction
x = 3 - 4
print(x) # Output: -1

# Multiplication
x = 3 * 4
print(x) # Output: 12

# Division
x = 3 / 4
print(x) # Output: 0.75

# Modulus
x = 7 % 3
print(x) # Output: 1

# Exponentiation
x = 3 ** 4
print(x) # Output: 81

# Floor division
x = 7 // 3
print(x) # Output: 2
```

It’s also important to note that Python follows the order of operations (PEMDAS) when evaluating arithmetic expressions.

PEMDAS stands for Parentheses, Exponents, Multiplication and Division, and Addition and Subtraction. It is the order in which Python (and most other programming languages and math systems) evaluates arithmetic operations in an expression.
1. Parentheses: Expressions within parentheses are evaluated first.
2. Exponents: Exponentiation (ie raising to a power) is done next.
3. Multiplication and Division (from left to right): These operations are done next, from left to right.
4. Addition and Subtraction (from left to right): These operations are done last, from left to right.

### 3.1.2 Comparison Operators

Comparison operators are an essential part of any programming language, and Python is no exception. These operators allow you to compare values and determine the relationship between them. The result of a comparison is a Boolean value, either True or False, which can be used to make decisions in your code. In Python, the following comparison operators are available:

`“==” (equal to), “!=” (not equal to), “>” (greater than), “<” (less than), “>=” (greater than or equal to), and “<=” (less than or equal to).` These operators can be used to compare numbers, strings, and even objects. It’s important to note that the use of comparison operators is a fundamental aspect of programming and understanding how to use them correctly is crucial for writing effective and efficient code.


| Operator    | Meaning    |Example|Result|
| --- | --- | --- | --- |
|  ==   | Equal to    | 3 == 2   | False   |
|`! =`|Not equal to|3 != 2|True|
|>|Greater than|3 > 2|True|
|<|Less than|3 < 2|False|
|>=|Greater than or equal to|3 >= 2|True|
|<=|Less than or equal to|3 <= 2|False|

```python
# Equal to
x = 3
y = 4
print(x == y) # Output: False

# Not equal to
x = 3
y = 4
print(x != y) # Output: True

# Greater than
x = 3
y = 4
print(x > y) # Output: False

# Less than
x = 3
y = 4
print(x < y) # Output: True

# Greater than or equal to
x = 3
y = 4
print(x >= y) # Output: False

# Less than or equal to
x = 3
y = 4
print(x <= y) # Output: True
```

### 3.1.3 Assignment Operator

In Python, the assignment operator is the “=” symbol. It is used to assign a value to a variable. For example, in the statement “x = 5”, the variable “x” is being assigned the value of 5. In addition to the basic assignment operator, there are a few other assignment operators that can be used to perform operations and assign the result to a variable in a single statement.

| Operator | Meaning                                                                                                                                                                      | Example | Result     |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- | ---------- |
| =        | Basic assignment: Assigns a value to a variable                                                                                                                              | x = 5   | x = 5      |
| +=       | Add and assign: which adds the right-hand side to the variable on the left-hand side and assigns the result to the variable.                                                 | x += 5  | x = x + 5  |
| -=       | Subtract and assign: which subtracts the right-hand side from the variable on the left-hand side and assigns the result to the variable.                                     | x -= 5  | x = x - 5  |
| `*=`     | Multiply and assign: which multiplies the variable on the left-hand side by the right-hand side and assigns the result to the variable                                       | x *= 5  | x = x * 5  |
| /=       | Divide and assign: which divides the variable on the left-hand side by the right-hand side and assigns the result to the variable.                                           | x /= 5  | x = x / 5  |
| //=      | Floor divide and assign: which performs floor division on the variable on the left-hand side by the right-hand side and assigns the result to the variable.                  | x //= 5 | x = x // 5 |
| %=       | Modulus and assign: which calculates the remainder of the variable on the left-hand side when divided by the right-hand side and assigns the result to the variable.         | x %= 5  | x = x % 5  |
| `**=`    | Exponent and assign: which raises the variable on the left-hand side to the power of the right-hand side and assigns the result to the variable.                             | x **= 5 | x = x ** 5 |
| &=       | Bitwise and assign: which performs bitwise and operation on the variable on the left-hand side by the right-hand side and assigns the result to the variable.                | x &= 5  | x = x & 5  |
| ^=       | Bitwise xor assign: which performs bitwise xor operation on the variable on the left-hand side by the right-hand side and assigns the result to the variable?                | x ^= 5  | x = x ^ 5  |
| `>>=`    | Bitwise right shift assign: which performs bitwise right shift operation on the variable on the left-hand side by the right-hand side and assigns the result to the variable | x >>= 5 | x = x >> 5 |
| <<=      | Bitwise left shift assign: which performs bitwise left shift operation on the variable on the left-hand side by the right-hand side and assigns the result to the variable.  | x <<= 5 | x = x << 5 |

It is important to note that the right-hand side of the operator must be a valid expression that can be evaluated to a value. Also, the above table is meant to give you an idea of the operations being performed and the resulting values, but in practice, you would need to assign the values to the variable and then perform the operations.

### 3.1.4 Logical Operators (Boolean Operators)

In Python, the logical operators are and, or, and not. These operators allow you to create boolean expressions, which evaluate to either True or False. The most common logical operators are given as follow: 
- and: returns True if both the expressions are true, otherwise False 
- or : returns True if at least one of the expressions is true, otherwise False.
- not : returns True if the expression is false, otherwise False.

```python
# and operator
if (x > 0) and (x < 10):
print(“x is a positive single-digit number.”)

# or operator
if (x < 0) or (x > 10):
print(“x is a negative number or a number greater than 10.”)

# not operator
if not (x == y):
print(“x is not equal to y.”)
```

Note that the and, or, and not keywords are used to perform logical operations in Python, as opposed to the symbols &, |, and ! commonly used in other programming languages.

### 3.1.5 Bitwise Operators

In Python, the bitwise operators are `&, |, ^, ~, <<, and >>`. These operators allow you to manipulate individual bits in an integer value. Let’s see in table below the common bitwise operators in Python with an example of how they are used :

| Operator | Name        | Example | Result |
| -------- | ----------- | ------- | ------ |
| &        | AND         | 5 & 3   | 1      |
| \|       | OR          | 5 \| 3  | 7      |
| ^        | XOR         | 5 ^ 3   | 6      |
| ~        | NOT         | ~5      | -6     |
| <<       | Left shift  | 5 << 2  | 20     |
| `>>`     | Right shift | 5 >> 2  | 1      |

Keep in mind that these operators only work on integers and the result is also an integer.

### 3.1.6 Special Operators

#### 3.1.6.1 Identity Operators

In Python, the identity operators are used to determining whether two objects are the same object. There are two identity operators:
- is: returns True if the objects are the same object, False otherwise
- is not: returns True if the objects are not the same object, False otherwise 

```python
x = [1, 2, 3]
y = [1, 2, 3]
z = x

# x and y are different objects
print(x is y) # Output: False
# x and z are the same object
print(x is z) # Output: True
# x and y are not the same object
print(x is not y) # Output: True
# x and z are the same object
print(x is not z) # Output: False
x = [1, 2, 3]
y = [1, 2, 3]
# x and y have the same content
print(x == y) # Output: True
# x and y are different objects
print(x is y) # Output: False
```

#### 3.1.6.2 Membership Operators

In Python, the membership operators are in and not in. These operators are used to test whether a value is found within a sequence (such as a string, tuple, or list) or not. The operator in returns True if the value is found in the sequence and False if it is not. The operator not in returns True if the value is not found in the sequence and False if it is.

```python
# Test if ‘a’ is in the string ‘abc’
‘a’ in ‘abc’ # True

# Test if ‘d’ is not in the string ‘abc’
‘d’ not in ‘abc’ # True

# Test if 1 is in the list [1, 2, 3]
1 in [1, 2, 3] # True

# Test if 4 is not in the list [1, 2, 3]
4 not in [1, 2, 3] # True

# Assign a string to a variable
s = ‘abc’
# Test if ‘a’ is in the string
‘a’ in s # True

# Assign a list to a variable
l = [1, 2, 3]

# Test if 2 is in the list
2 in l # True
```

