## **Class 10 Python Practicals Notes (Expanded)**

### 1. **Introduction to Python**
- **What is Python?**
  Python is a high-level, interpreted programming language known for its simplicity and readability. It allows for rapid application development and supports multiple programming paradigms.
  
- **Python Features:**
  - **Simple and Easy to Learn**: Python’s syntax is clear and concise.
  - **Cross-platform**: Runs on different operating systems (Windows, Mac, Linux).
  - **Open Source**: Free to use and distribute.
  - **Rich Standard Library**: Provides modules and functions to do many things.
  - **Interpreted**: Python code is executed line by line, making debugging easier.
  - **Dynamic Typing**: You don't need to declare the type of variable, Python detects it automatically.
  
### 2. **Python Syntax**
- **Indentation**: Python uses indentation (spaces or tabs) to define code blocks. Proper indentation is essential for the program to work correctly.
  
  ```python
  if 5 > 2:
      print("Five is greater than two!")
  ```

- **Comments**: Used to explain the code. Comments begin with `#`.
  
  ```python
  # This is a comment
  print("Hello, World!")  # This is also a comment
  ```

- **Multiline Comments**: Can be created using triple quotes (`'''` or `"""`).
  
  ```python
  '''
  This is a
  multiline comment
  '''
  ```

### 3. **Python Variables and Data Types**
- **Variables**: Store values that can be used and manipulated later.
  ```python
  x = 10       # integer
  y = 3.14     # float
  name = "Alice"  # string
  is_student = True  # boolean
  ```

- **Rules for naming variables**:
  - Variables can have letters, numbers, and underscores, but cannot start with a number.
  - Case-sensitive: `age` and `Age` are different variables.
  - Avoid using Python keywords like `if`, `else`, `for`, etc.

- **Data Types**:
  - **int**: Whole numbers without a decimal point (e.g., `5`, `-10`).
  - **float**: Numbers with a decimal point (e.g., `3.14`, `-0.99`).
  - **str**: Strings (text enclosed in quotes) (e.g., `"Hello"`).
  - **bool**: Boolean values, either `True` or `False`.

  ```python
  print(type(x))  # Output: <class 'int'>
  print(type(y))  # Output: <class 'float'>
  ```

### 4. **Basic Input and Output**
- **Printing output**:
  - `print()` function is used to display output to the screen.
  
  ```python
  print("Hello, World!")  # Prints Hello, World!
  print("The value of x is", x)  # Prints The value of x is 10
  ```

- **Taking input**:
  - `input()` function is used to take input from the user. Input is always read as a string, so it needs to be converted to the desired data type.
  
  ```python
  name = input("Enter your name: ")
  age = int(input("Enter your age: "))  # Convert to integer
  print("Hello", name, ", you are", age, "years old.")
  ```

### 5. **Operators in Python**
- **Arithmetic Operators**:
  - `+`: Addition
  - `-`: Subtraction
  - `*`: Multiplication
  - `/`: Division (floating-point division)
  - `//`: Floor division (returns the integer part of the division)
  - `%`: Modulus (remainder)
  - `**`: Exponentiation (power)

  ```python
  a = 5
  b = 2
  print(a + b)  # 7
  print(a // b)  # 2 (integer division)
  print(a ** b)  # 25 (5 raised to the power 2)
  ```

- **Relational/Comparison Operators**:
  - `==`: Equal to
  - `!=`: Not equal to
  - `>`: Greater than
  - `<`: Less than
  - `>=`: Greater than or equal to
  - `<=`: Less than or equal to

  ```python
  x = 10
  y = 20
  print(x > y)  # False
  print(x == y)  # False
  ```

- **Logical Operators**:
  - `and`: True if both conditions are true.
  - `or`: True if at least one condition is true.
  - `not`: Reverses the result, True becomes False, and vice versa.

  ```python
  age = 18
  has_ID = True
  print(age >= 18 and has_ID)  # True
  ```

### 6. **Control Structures (Conditional Statements)**
- **If-Else Statements**: These allow decisions to be made based on conditions.
  
  ```python
  if age >= 18:
      print("You are an adult.")
  else:
      print("You are a minor.")
  ```

- **Elif**: Used when there are multiple conditions to check.

  ```python
  marks = 85
  if marks >= 90:
      print("Grade A")
  elif marks >= 80:
      print("Grade B")
  elif marks >= 70:
      print("Grade C")
  else:
      print("Grade D")
  ```

### 7. **Loops in Python**
- **For Loop**: Used to iterate over a sequence like a list, tuple, or string.
  
  ```python
  for i in range(5):
      print(i)  # Output: 0 1 2 3 4
  ```

  **Range Function**:
  - `range(5)` generates numbers from 0 to 4.
  - `range(start, stop, step)` allows specifying a starting point and step size.
  
  ```python
  for i in range(2, 10, 2):
      print(i)  # Output: 2 4 6 8
  ```

- **While Loop**: Repeats the block of code as long as the condition is `True`.
  
  ```python
  count = 0
  while count < 5:
      print(count)
      count += 1
  ```

### 8. **Lists in Python**
- **List**: A collection of items, ordered and mutable, enclosed in square brackets `[]`.

  ```python
  fruits = ["apple", "banana", "cherry"]
  print(fruits[0])  # Output: apple
  fruits.append("orange")  # Add to the list
  fruits.remove("banana")  # Remove from the list
  ```

- **List Operations**:
  - `len()`: To find the length of the list.
  - `append()`: Add an element to the end.
  - `remove()`: Remove an element.
  - `sort()`: Sorts the list.
  - `reverse()`: Reverses the order of the list.

  ```python
  fruits = ["apple", "cherry", "banana"]
  print(len(fruits))  # Output: 3
  fruits.sort()  # Sort alphabetically
  print(fruits)  # Output: ['apple', 'banana', 'cherry']
  ```

### 9. **Functions in Python**
- **Defining Functions**: Functions are defined using the `def` keyword and can be called when needed.

  ```python
  def greet():
      print("Hello, World!")
  
  greet()  # Calling the function
  ```

- **Function with Parameters**:
  ```python
  def add(a, b):
      return a + b
  
  result = add(5, 3)
  print(result)  # Output: 8
  ```

### 10. **Error Handling in Python**
- **Try-Except Block**: Used to handle exceptions (runtime errors) in the program.

  ```python
  try:
      a = int(input("Enter a number: "))
      print(10 / a)
  except ZeroDivisionError:
      print("Division by zero is not allowed.")
  except ValueError:
      print("Invalid input! Please enter a number.")
  ```

### 11. **Common Python Programs for Practicals**

- **Program to find the largest of three numbers**:
  ```python
  a = int(input("Enter first number: "))
  b = int(input("Enter second number: "))
  c = int(input("Enter third number: "))

  if a >= b and a >= c:
      print(a, "is the largest")
  elif b >= a and b >= c:
      print(b, "is the largest")
  else:
      print(c, "is the largest")
  ```

- **Program to check whether a number is even or odd**:
  ```python
  num = int(input("Enter a number: "))
  if num % 2 == 0:
      print(num

, "is even")
  else:
      print(num, "is odd")
  ```

- **Program to find the sum of the first N natural numbers**:
  ```python
  n = int(input("Enter a number: "))
  sum_n = n * (n + 1) // 2
  print("Sum of first", n, "natural numbers is", sum_n)
  ```

- **Program to find the factorial of a number**:
  ```python
  def factorial(n):
      if n == 0 or n == 1:
          return 1
      else:
          return n * factorial(n-1)

  num = int(input("Enter a number: "))
  print("Factorial of", num, "is", factorial(num))
  ```

- **Program to generate the Fibonacci sequence**:
  ```python
  def fibonacci(n):
      a, b = 0, 1
      for _ in range(n):
          print(a, end=" ")
          a, b = b, a + b

  n = int(input("Enter the number of terms: "))
  fibonacci(n)
  ```

### 12. **Miscellaneous Programs**

- **Program to check if a number is prime**:
  ```python
  num = int(input("Enter a number: "))
  if num > 1:
      for i in range(2, num):
          if num % i == 0:
              print(num, "is not a prime number")
              break
      else:
          print(num, "is a prime number")
  else:
      print(num, "is not a prime number")
  ```

- **Program to reverse a string**:
  ```python
  string = input("Enter a string: ")
  print("Reversed string is:", string[::-1])
  ```
