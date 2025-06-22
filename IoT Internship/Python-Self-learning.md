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
###🧾 Task: You and your 2 friends go to a restaurent. The total bill is 1234 rupees. How much should each pay?
```
a = 1234
b = 3
print("Money each person should pay:", a/b)
```

##🧵 Strings in Python
-Text data in Python.
-Double or single quotes can be used.

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







> 🚧 This is a work in progress. Will be updated with more notes later.
