# Python Logic Building Questions 

## 1. Even or Odd

```python
num = int(input("Enter number: "))

if num % 2 == 0:
    print("Even")
else:
    print("Odd")
```

## 2. Reverse a String

```python
text = "automation"
print(text[::-1])
```

## 3. Count Characters in String

```python
text = "sdet"
count = 0

for char in text:
    count += 1

print("Length:", count)
```

## 4. Find Largest of 3 Numbers

```python
a = 10
b = 25
c = 15

largest = max(a, b, c)
print("Largest:", largest)
```

## 5. FizzBuzz Program

Print numbers from 1 to 100 with special rules:

- Multiples of 3 → "Fizz"  
- Multiples of 5 → "Buzz"  
- Multiples of both → "FizzBuzz"

```python
for num in range(1, 101):
    if num % 3 == 0 and num % 5 == 0:
        print("FizzBuzz")
    elif num % 3 == 0:
        print("Fizz")
    elif num % 5 == 0:
        print("Buzz")
    else:
        print(num)
```

---

## 6. Count Vowels in a String

```python
text = "automation engineer"
vowels = "aeiou"
count = 0

for char in text.lower():
    if char in vowels:
        count += 1

print("Vowel count:", count)
```

- `text.lower()` ensures uppercase vowels are also counted  
- `count += 1` increases the counter for each vowel found  

---

## 7. Find Factorial of a Number

Factorial of a number is the product of all positive integers up to that number.

Example:  
5! = 5 × 4 × 3 × 2 × 1 = 120

```python
num = 5
fact = 1

for i in range(1, num + 1):
    fact *= i

print("Factorial:", fact)
```

The loop multiplies numbers from 1 to `num`.

---

## 8. Check if a Word is a Palindrome

A palindrome reads the same forward and backward.

```python
word = "madam"

if word == word[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")
```

- `[::-1]` reverses the string  
- The program compares the original word with the reversed version  

---




