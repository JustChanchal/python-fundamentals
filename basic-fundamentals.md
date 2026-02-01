# Python Fundamentals(Basics)

Python provides several built-in data types that are used frequently in everyday programming.

## Common Python Data Types 

| Data Type | Description | Example |
|-----------|-------------|---------|
| `int` | Integer numbers | `10`, `-5` |
| `float` | Decimal numbers | `3.14`, `-0.01` |
| `str` | Text / String | `"Hello"` |
| `bool` | Boolean (True/False) | `True`, `False` |
| `list` | Ordered, mutable collection | `[1, 2, 3]` |
| `tuple` | Ordered, immutable collection | `(1, 2, 3)` |
| `dict` | Key-value pairs | `{"name": "John"}` |
| `set` | Unordered unique values | `{1, 2, 3}` |

---

# Operators & Conditions

Operators allow you to perform operations on variables and values.

## Arithmetic Operators

| Operator | Meaning | Example |
|----------|---------|---------|
| `+` | Addition | `a + b` |
| `-` | Subtraction | `a - b` |
| `*` | Multiplication | `a * b` |
| `/` | Division | `a / b` |

## Comparison Operators

| Operator | Meaning | Example |
|----------|---------|---------|
| `==` | Equal to | `a == b` |
| `!=` | Not equal to | `a != b` |
| `>` | Greater than | `a > b` |
| `<` | Less than | `a < b` |

## Logical Operators

| Operator | Meaning | Example |
|----------|---------|---------|
| `and` | True if both conditions are true | `a > 5 and b < 10` |
| `or` | True if at least one condition is true | `a > 5 or b < 10` |
| `not` | Reverses the result | `not(a > b)` |

---

## Example Code for Operators

```python
a = 10
b = 20

print(a < b)  # True
print(a == 10 and b == 20)  # True
```

# Decision Making in Python (if-elif-else)

Decision-making statements allow a program to execute different blocks of code based on conditions.

---

## Basic `if` Statement 

Runs a block of code **only if the condition is True**.

```python
age = 20

if age >= 18:
    print("You are an adult.")
```

---

## `if-else` Statement

Executes one block if the condition is **True**, otherwise runs another block.

```python
age = 16

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible")
```

---

## `if-elif-else` Statement

Used when you need to check **multiple conditions**.

```python
marks = 75

if marks >= 90:
    print("Grade A")
elif marks >= 70:
    print("Grade B")
elif marks >= 50:
    print("Grade C")
else:
    print("Fail")
```

Python checks conditions **top to bottom** and stops when one is True.

---

## Nested `if` Statements

An `if` statement inside another `if`.

```python
age = 25
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote")
    else:
        print("Not a citizen")
else:
    print("Too young to vote")
```

---

## Using Logical Operators in Conditions

You can combine multiple conditions using `and`, `or`, and `not`.

```python
age = 22
has_id = True

if age >= 18 and has_id:
    print("Entry allowed")
else:
    print("Entry denied")
```

---

## Short-Hand If-Else

A compact way to write simple conditions.

```python
age = 18
status = "Adult" if age >= 18 else "Minor"
print(status)
```

---

## Important Rules

- Indentation is mandatory in Python  
- Use a colon `:` after `if`,`elif`, and, `else`  
- Conditions must return **True** or **False**  
- Only **one** `else` is allowed per `if` block  

---

## Example Code

```python
number = 7

if number % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```


