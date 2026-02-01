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
