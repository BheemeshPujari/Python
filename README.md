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
String is a data type which is an immutable ordered sequence of characters
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

2. Concatenation with Space
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
len() is a built-in function that returns the object's length.  
The length of a string is the number of characters in the string. This will always be an integer.
len only works on a "sequence (such as a string, bytes, tuple, list, or range) or a collection (such as a dictionary, set, or frozen set),
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
# String Methods in Python

In Python, methods are functions that are associated with a specific data type and are called using dot notation. They operate on the data of that type and can take additional arguments. Methods are available for various data types, and here we'll focus on string methods.

## Common String Methods


The `islower()` method checks if all the characters in a string are lowercase.

#### islower()
```python
my_string = "Rama"
print(my_string.islower())
# Output: False
```

#### count(substring)
```python
my_string = "messi ronaldo swift ronaldo"
print(my_string.count('ronaldo'))
# Output: 2
```

#### find(substring)
```python
my_string = "rama"
print(my_string.find('am'))
# Output: 1
```
#### The format() String Method

##### Example 1
```python
print("Krishna has {} cards".format(13))
# Output: Krishna has 13balloons
```

##### Example 2
```python
sport = "football"
action = "watch"
print("Does your son {} {}?".format(action,sport))
# Output: Does your son watch football?
```

##### Example 3
```python
maria_string = "arjun loves {} and {}"
print(maria_string.format("math", "cinema"))
# Output: arjun loves math and cinema
```
## String Splitting in Python

### The `split()` Method

The `split()` method in Python is used to split a string into a list of substrings. It takes two optional arguments: `sep` (separator) and `maxsplit`.

### Example:

```python
# Example String
sentence = "The quick brown fox jumps over the lazy dog."
```
##### Basic split (default separator is whitespace)
```python
word_list = sentence.split()
print(word_list)
# Output: ['The', 'quick', 'brown', 'fox', 'jumps', 'over', 'the', 'lazy', 'dog.']
```

##### Split with a specific separator and maxsplit  
Here's how the splits occur:
'The' (first word before the first space)
'quick' (second word after the first space)
'brown' (third word after the second space)
'Fox jumps over the lazy dog.' (the remaining part after the third space)
```python
phrase_list = sentence.split(' ', 3)
print(phrase_list)
# Output: ['The', 'quick', 'brown', 'fox jumps over the lazy dog.']
```

##### Split using period as a separator
The split() method identifies the period as the separator and creates substrings wherever it encounters a period. Therefore, each occurrence of a period in the original string results in a split.  
So, wherever a full stop occurs in the original string, a split happens, and the resulting list contains the segments between those full stops.
```python
sentence_parts = sentence.split('.')
print(sentence_parts)
# Output: ['The quick brown fox jumps over the lazy dog', '']
```
##### with no separators but having a maxsplit argument 
```Python
wordsplit = sentence.split(None, 3)
print(wordsplit)
# Output :['The', 'quick', 'brown', 'fox jumps over the lazy dog.']
```
### Common String Methods

| Method          | Description                                                                                                    | Example                                           |
|-----------------|----------------------------------------------------------------------------------------------------------------|---------------------------------------------------|
| `capitalize()`  | Returns a copy of the string with its first character capitalized and the rest lowercase.                      | `'hello'.capitalize()` => `'Hello'`                |
| `casefold()`    | Returns a casefolded version of the string, suitable for case-insensitive comparisons.                         | `'Hello'.casefold()` => `'hello'`                  |
| `count(sub)`    | Returns the number of occurrences of a substring in the string.                                                 | `'apple'.count('p')` => `2`                        |
| `endswith(suffix)` | Checks if the string ends with a specified suffix and returns `True` or `False`.                                | `'world'.endswith('ld')` => `True`                 |
| `find(sub)`     | Returns the lowest index of the substring if found, -1 otherwise.                                               | `'hello'.find('lo')` => `3`                        |
| `rfind(sub)`    | Returns the highest index of the substring if found, -1 otherwise.                                              | 'hello'.rfind('lo') => 3                           |
| `isalnum()`     | Returns `True` if all characters in the string are alphanumeric (letters or numbers), `False` otherwise.       | `'abc123'.isalnum()` => `True`                     |
| `isalpha()`     | Returns `True` if all characters in the string are alphabetic (letters), `False` otherwise.                    | `'abc'.isalpha()` => `True`                        |
| `isdigit()`     | Returns `True` if all characters in the string are digits, `False` otherwise.                                  | `'123'.isdigit()` => `True`                        |
| `islower()`     | Returns `True` if all cased characters in the string are lowercase, `False` otherwise.                         | `'hello'.islower()` => `True`                      |
| `isupper()`     | Returns `True` if all cased characters in the string are uppercase, `False` otherwise.                         | `'HELLO'.isupper()` => `True`                      |
| `lower()`       | Returns a copy of the string with all case characters converted to lowercase.                                 | `'Hello'.lower()` => `'hello'`                    |
| `upper()`       | Returns a copy of the string with all case characters converted to uppercase.                                 | `'hello'.upper()` => `'HELLO'`                    |
| `replace(old, new)` | Returns a copy of the string with occurrences of substring `old` replaced with `new`.                          | `'apple'.replace('p', 'b')` => `'abble'`           |
| `split(separator)` | Splits the string into a list of substrings using the specified separator and returns the list.                | `'apple, orange,banana'.split(',')` => `['apple', 'orange', 'banana']` |
| `startswith(prefix)` | Checks if the string starts with a specified prefix and returns `True` or `False`.                              | `'hello'.startswith('he')` => `True`               |
| `strip()`       | Returns a copy of the string with leading and trailing whitespace removed.                                     | `'   hello   '.strip()` => `'hello'`               |
| `format(args)`  | Formats the string by replacing placeholders with values.                                                      | `"{} has {} apples".format('John', 3)` => `'John has 3 apples'` |


###  * floats have the is_integer() method which strings don't have.
###  * \n is a special sequence of characters that causes a line break (a new line).

