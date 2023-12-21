# Python
Just a practice and points that are discussed in the tutorial 
## Data Types and operators 
Print() - is an inbuilt function that displays the given input values as an output.
### Arithmetic Operators
| Operator symbol| Operation | 
| -------- | -------- |
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |
| //| Integer Division(Divides and rounds down to the nearest integer) |
| %| Modulo (the remainder after dividing)|
|** | power |
| ^| Bitwise XOR |

```python
print("The Integer Division of ", 3 // 2)

<!-- Output:
The Integer Division of  1
-->
```
***BODMAS Rule is applied for preference among these operators***
-> Bracket of Division, Multiplication, Addition, subtraction
# Variables
```
Arjun_k = 1
```
Here Arjun_k is the name of the variable that we are using and 1 is the value that is being assigned, simply here we declared a variable and assigned a value to it

"=" is the assignment operator, Generally it does the thing to assign the item on the right to the name on the left.  
If we try to access an undeclared variable, we get an error.
```python
Arjun_k = 1
Bheem_p = Arjun_k
# Here we are assigning the value of Arjun_k to the Bheem_p
```

``` python
Arjun_k = 1
Bheem_p = Nakul_r
print(Bheem_p)

<!-- Output:
NameError: name 'Nakul_r' is not defined
-->
```

The Naming of variables cannot start with a number or underscore(_).  
Also, we cannot use Reserved Words or BUIT-IN Identifiers   
All the letters need to be in lowercase and underscore to separate words.


### Assignment Operators in Python

| Operator | Description                   | Example                      |
|----------|-------------------------------|------------------------------|
| `=`      | Assignment Operator           | `x = 42`                     |
| `+=`     | Addition Assignment           | `y += 5`  (Equivalent to `y = y + 5`)   |
| `-=`     | Subtraction Assignment        | `z -= 8`  (Equivalent to `z = z - 8`)   |
| `*=`     | Multiplication Assignment     | `w *= 3`  (Equivalent to `w = w * 3`)   |
| `/=`     | Division Assignment           | `p /= 2`  (Equivalent to `p = p / 2`)   |
| `%=`     | Remainder Assignment          | `q %= 7`  (Equivalent to `q = q % 7`)   |
| `**=`    | Exponent Assignment           | `r **= 4` (Equivalent to `r = r ** 4`)  |

### Python Keywords

| Keyword   | Explanation                                      | Example                                       |
|-----------|--------------------------------------------------|-----------------------------------------------|
| `False`   | Boolean value representing false                | `flag = False`                                |
| `await`   | Used in asynchronous programming                | `async def example_function(): await something`|
| `else`    | Executes when the `if` condition is not true     | `if x > 0: print("Positive") else: print("Non-positive")` |
| `import`  | Used to import modules                           | `import math`                                 |
| `pass`    | Placeholder for future code                      | `def my_function(): pass`                     |
| `None`    | Represents the absence of a value               | `result = None`                               |
| `break`   | Exits the loop prematurely                       | `for i in range(5): if i == 3: break`         |
| `except`  | Catches exceptions in a `try` block             | `try: some_code() except Exception as e: handle_error(e)` |
| `in`      | Checks if a value is present in a sequence      | `if item in my_list: print("Item is present")` |
| `raise`   | Raises an exception                             | `raise ValueError("This is a custom error")` |
| `True`    | Boolean value representing true                 | `flag = True`                                |
| `class`   | Defines a class                                 | `class MyClass: def __init__(self): pass`     |
| `finally` | Executes code, regardless of whether an exception occurs or not | `try: some_code() finally: cleanup_code()` |
| `is`      | Checks for object identity                      | `if x is None: print("x is None")`           |
| `return`  | Exits a function and returns a value            | `def add(x, y): return x + y`                |
| `and`     | Logical AND                                     | `if x > 0 and y > 0: print("Both positive")` |
| `continue`| Skips the rest of the loop's code and continues with the next iteration | `for i in range(5): if i == 3: continue` |
| `for`     | Used for looping over an iterable               | `for item in my_list: print(item)`           |
| `lambda`  | Creates an anonymous function (lambda function) | `square = lambda x: x**2`                    |
| `try`     | Implements error handling in a block of code    | `try: some_code() except SomeError: handle_error()` |
| `as`      | Renames a module or variable in import statement | `import math as m`                           |
| `def`     | Defines a function                              | `def greet(name): print(f"Hello, {name}!")`  |
| `from`    | Used in import statements to import specific items | `from module import function`               |
| `nonlocal`| Declares a variable to be nonlocal in nested functions | `def outer(): x = 10 def inner(): nonlocal x; x = 20` |
| `while`   | Loops while a certain condition is true         | `while x < 5: print(x); x += 1`             |
| `assert`  | Asserts that a condition is true                | `assert x > 0, "x should be positive"`      |
| `del`     | Deletes an object or a variable                | `del my_list[2]`                             |
| `global`  | Declares a variable to be global                | `global x; x = 10`                          |
| `not`     | Logical NOT                                     | `if not condition: print("Condition is not true")` |
| `with`    | Simplifies resource management using a context manager | `with open("file.txt", "r") as file: content = file.read()` |
| `async`   | Declares an asynchronous function               | `async def async_function(): await something`|
| `elif`    | Used in conditional statements as an "else if"  | `if x > 0: print("Positive") elif x < 0: print("Negative")` |
| `if`      | Executes code based on a condition              | `if x > 0: print("Positive")`               |
| `or`      | Logical OR                                      | `if x > 0 or y > 0: print("At least one is positive")` |
| `yield`   | Pauses the execution of a generator function and yields a value | `def generator(): yield 1; yield 2` |

## Integers and Floats
Even when the integers are perfectly divisible the output will be a float.
``` python 
print(9/3)
# The output will be 3.0
```

``` python
x = 9/3
print(type(x))
#  output is <class 'float'>
```

type() is a built-in function that returns the type of the object.  

```python
print(.2+ .2 + .2 == .6)
# output will be False
```
```python
print(7/0)
<!-- Output:
ZeroDivisionError: division by zero
-->
```

Even if a statement or expression is syntactically correct, it may cause an error when an attempt is made to execute it. Errors detected during execution are called **exceptions**.  
A 'Syntax Error' is a problem detected when Python checks the code before it runs it.

## Booleans, Comparison Operators, and Logical Operators
A Bool is a data type that can have a value True or False.

### Comparison Operators

| Symbol | Use Case | Bool  | Operation                  |
|--------|----------|-------|----------------------------|
| <      | 4 < 8    | True  | Less Than                    |
| >      | 6 > 2    | True  | Greater Than                 |
| <=     | 5 <= 5   | True  | Less Than or Equal To        |
| >=     | 2 >= 7   | False | Greater Than or Equal To     |
| ==     | 3 == 3   | True  | Equal To                     |
| !=     | 4 != 7   | True  | Not Equal To                 |

### Logical Operators

| Logical Use            | Bool  | Operation                                   |
|------------------------|-------|---------------------------------------------|
| 4 < 8 and 4 == 4      | True  | `and` - Evaluates if all provided statements are True |
| 6 > 2 or 6 == 6       | True  | `or` - Evaluates if at least one of many statements is True |
| not 4 < 8             | False | `not` - Flips the Bool Value                 |

### Strings
String is a data type which is immutable ordered sequence of characters
Strings in Python are represented as the variable type `str`. You can define a string with either double quotes (`"`) or single quotes (`'`). If the string itself contains one of these quote characters, you can use the other type of quote to define the string.
```python
print(len("arjun_krishna"))
<!-- Output: 13
-->
# Examples of defining strings
my_string = 'this is a string!'
my_string2 = "this is also a string!!!"

# Example with an escaped quote
this_string = 'Simon\'s skateboard is in the garage.'
print(this_string)
# Output: Simon's skateboard is in the garage.
```
# String Operations

1. Concatenation
```python
first_word = 'Happy'
second_word = 'world'
print(first_word + second_word)
<!-- Output: Happyworld
-->
```

2.Concatenation with Space
```python
print(first_word + ' ' + second_word)
<!-- Output: Happy world
-->
```

3. Repetition
```python
print(first_word * 5)
<!--Output: HappyHappyHappyHappyHappy
-->
```

4. Length 
len() is a built-in function that returns the length of the object.  
The length of a string is the number of characters in the string. This will always be an integer.
```python
print(len(first_word))
<!--Output: 5
-->
```

5. String Indexing
```python
print(first_word[0])
<!--Output: H
-->

print(first_word[-1])
<!--Output: y
-->
```
