# Classes & Objects in Python

Classes and objects are the foundation of **Object-Oriented Programming (OOP)** in Python.

A **class** is like a blueprint.  
An **object** is a real thing created from that blueprint.

---    

## 1. Basic Class

```python
class Car:
    def start(self):
        print("Car started")

my_car = Car()
my_car.start()
```

### Explanation

- `Car` → **Class** (blueprint)
- `my_car` → **Object** (instance of the class)
- `start()` → **Method** (function inside a class)

We create an object using:
```python
my_car = Car()
```

We call a method using:
```python
my_car.start()
```

---

## 2. Constructor (`__init__`)

A constructor runs **automatically** when an object is created.

```python
class User:
    def __init__(self, username):
        self.username = username

    def greet(self):
        print("Hello", self.username)

u1 = User("Chanchal")
u1.greet()
```

### Explanation

- `__init__` is a **special method** (constructor)
- It is used to **initialize data** when the object is created
- `self.username = username` stores the value inside the object

### What is `self`?

`self` refers to the **current object**.

It allows each object to store its own data.

Example:
- `u1.username` → `"Chanchal"`

---

## 3. Real Automation Example

This is similar to how **Page Object Model (POM)** works in automation.

```python
class LoginPage:
    def __init__(self, page):
        self.page = page

    def enter_username(self, username):
        print("Typing username:", username)

    def enter_password(self, password):
        print("Typing password:", password)

    def click_login(self):
        print("Clicking login button")
```

### Explanation

- `LoginPage` is a class representing a **web page**
- Each method represents an **action on the page**
- `self.page` would store the browser/page object (like Selenium or Playwright)

This keeps test code **clean and reusable**.

---

