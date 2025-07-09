# 🐍 Python Basics – My Notes

## 1. Introduction to Python

- Python is a high-level, easy-to-learn programming language.
- Used in web development, automation, data science, and IoT.
- Great for beginners.

### 📱 Examples of IoT Devices Using Python:
- Smart light automation using Raspberry Pi
- Temperature sensor reading

### 💻 Example Code:

```python
print("Hello, Python!")

Output
Hello, Python!
```

## 2. Variables and Data Types

- A variable is like a container used to store data in Python.
- You can give it any name and it holds numbers, text, or more.

### 🧪 Syntax:
```python
variable_name = value
```
### Example:
x = 10
name = "asha"
pi = 3.14
is_active = True

### 🔠 Data Types

| Type     | Example   | Description             |
|----------|-----------|-------------------------|
| Integer  | 5         | Whole number            |
| Float    | 3.14      | Decimal number          |
| String   | "hello"   | Text or inside quotes   |
| Boolean  | True/False| True or False values    |

### ⚠️ Things to Remember

- Python is **case sensitive** (e.g., `Name` and `name` are different).
- Strings must be inside **quotes** (either single `'` or double `"`).
- You **don’t have to declare** the data type — Python figures it out automatically.


### Code Examples
```age = 21
print("My age is", age)
# Output: My age is 21
```
```
name = "Asha"
print("Hello", name)
# Output: Hello Asha
```
```
name = input("What's your name?")
print("Nice to meet you,", name + "!")
# Output:What's your name? Lakshmi
Nice to meet you, Lakshmi!
```
### Program with types
```
name = "lakshmi"
age = 20
height = 5.4
is_student = True
print("Name:", name)
print("Age:", age)
print("Height:", height)
print("Student:", is_student)
print("Type of name:", type(name))
print("Type of age:", type(age))
print("Type of height:", type(height))
print("Type of is_student:", type(is_student))
```
# Output:
```
Name: lakshmi
Age: 20
Height: 5.4
Student: True
Type of name: <class 'str'>
Type of age: <class 'int'>
Type of height: <class 'float'>
Type of is_student: <class 'bool'>
```

🔄 Type Conversion
Change a value from one type to another.

Code 1:
```
age = "25"
print("Before conversion:", type(age))
age = int(age)
print("After conversion:", type(age))
```
Code 2:
```
pi = 3.14
pi_str = str(pi)
print("Pi as string:", pi_str)
print("Type of pi_str:", type(pi_str))
```
🧮 Mini Task
Use type conversion in a program to calculate age after 10 years.

Incorrect Code:
```
age = input("Enter your age:")
future_age = age + 10  # ❌ will not work because age is a string
```
Correct Code:
```
age = input("Enter your age:")
age = int(age)
future_age = age + 10
print("Age in 10 years is", future_age)
```
##➕ Topic: Basic Math Operations
| Operator | Meaning             |
| -------- | ------------------- |
| `+`      | Addition            |
| `-`      | Subtraction         |
| `*`      | Multiplication      |
| `/`      | Division            |
| `//`     | Floor division      |
| `%`      | Modulus (remainder) |
| `**`     | Exponentiation      |


### Code Example:
```
a = 10
b = 3
print("addition:", a + b)
print("subtraction:", a - b)
print("multiplication:", a * b)
print("division:", a / b)
print("floor division:", a // b)
print("modulus:", a % b)
print("exponentiation:", a ** b)
```
### Output:
```
addition: 13
subtraction: 7
multiplication: 30
division: 3.33
floor division: 3
modulus: 1
exponentiation: 1000
```
### 🧾 Task: You and your 2 friends go to a restaurent. The total bill is 1234 rupees. How much should each pay?
```
a = 1234
b = 3
print("Money each person should pay:", a/b)
```
---
## 🧵 Strings in Python
- Text data in Python.
- Double or single quotes can be used.

Code Examples:
```
name = "lakshmi"
# Joining
print("Hello", name)
# Length of string
print(len(name))
# Accessing characters
print(name[0])   # First character
print(name[-1])  # Last character
# Slicing
print(name[0:3])  # From 0 to 2
# Changing case
print(name.upper())
print(name.lower())
```
---

## 📌 Accessing Characters
- Indexing starts at 0.
- Negative indexing starts from -1.

L a k s h m i

0 1 2 3 4 5 6

-7 -6 -5 -4 -3 -2 -1


```python
word = "lakshmi"
print(word[0])   # Output: l
print(word[-1])  # Output: i
```

---


## ✂️ Slicing Strings

- Slicing means getting a part of the string.

- string[start_index:end_index]

- It includes start_index but not end_index.

 ``` 
word = "Lakshmi"
print(word[0:3])   # Lak
print(word[2:5])   # ksh
print(word[:4])    # Laks
print(word[3:])    # shmi
```


## 🔠 String Functions and Slicing Examples

```
name = "lakshmi"
print("hello" + name)         # hellolakshmi
print(len(name))              # 7
print(name[-1])               # i
print(name[1])                # a
print(name[2:7])              # kshmi
print(name[0:5])              # laksh
print(name[:4])               # laks
print(name[3:])               # shmi
print(name.upper())          # LAKSHMI
print(name.lower())          # lakshmi
```

### ✅ Make only one letter uppercase (2nd letter):

```
word = "lakshmi"
new_word = word[0] + word[1].upper() + word[2:]
print(new_word)  # Output: lAkshmi
```

### ✅ Make 4th character uppercase:

```
word = "lakshmi"
index = 3
new_word = word[:index] + word[index].upper() + word[index+1:]
print(new_word)
```

---

## ✅ Conditional Statements

### 1. if statement

```
age = 20
if age >= 18:
    print("You're an adult")
```

### 2. if with input()

```
age = input("My age is: ")
age = int(age)
if age >= 18:
    print("You are an adult")
```
### 3. if + else

```
age = 16
if age >= 18:
    print("You're an adult")
else:
    print("You're a minor")
``` 
### 4. elif (else if)

```
age = 70
if age < 18:
    print("You're a minor")
elif age < 60:
    print("You're an adult")
else:
    print("You're a senior citizen")
```
---
## 🧪 Practice Questions

### Q1: Check even or odd

```
number = input("Enter the number:")
number = int(number)
if number % 2 == 0:
    print("The number is even")
else:
    print("The number is odd")
```

### Q2: Grading System

```
mark = int(input("Enter your marks:"))
if mark >= 90:
    print("A grade")
elif 75 <= mark <= 89:
    print("B grade")
elif 60 <= mark <= 74:
    print("C grade")
else:
    print("FAIL")
```

### Q3: License Eligibility

```
age = int(input("Enter your age:"))
if age >= 18:
    print("eligible")
else:
    print("not eligible")
```

### Q4: Password Check

```
password = input("Enter your password: ")
if password == "lakshmi123":
    print("ACCESS GRANTED")
else:
    print("ACCESS DENIED")
```
























> 🚧 This is a work in progress. Will be updated with more notes later.
