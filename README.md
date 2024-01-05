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
6. String Slicing 
```python
hello_world = "Hello World"
print(hello_world[6:9])
# output: Wor
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

## Data Structures

### 1. Lists and Membership Operators.
 A List is a data structure in Python that is a mutable ordered sequence of elements.
 A List is defined in square brackets and always holds other data which are separated by commas, And this data could be a mix of any other data type.  
In Python, a list is a versatile data structure that can store a collection of items. Each item in a list can be of a different data type, allowing flexibility in handling various types of information.

```python
# Defining a List
list1 = ["month", "December", 3, 6.46, False]
```

#### Getting the Length of the List
The len() function is used to find the length of the list, which is the number of elements it contains.
```python
print("Length of the List:", len(list1))
```

#### Accessing Elements in the List
List indexing starts from 0, so list1[0] accesses the first element, and list1[-1] accesses the last element.  
```python
print("First Element:", list1[0])    # Output: month
print("Last Element:", list1[-1])    # Output: False
```

#### Attempting to Access an Index Beyond List Length
# This will result in an IndexError
```python
print(list1[len(list1)])  # output: IndexError: list index out of range 
```
#### Accessing the Last Element Safely
Attempting to access an index beyond the length of the list (list1[len(list1)]) will result in an index error. To avoid this, you can use list1[len(list1)-1] to safely access the last element.
```python
print("Last Element (Safe):", list1[len(list1)-1])
```
*** Lists are similar to strings, both support the len() function, slicing and indexing.  
length of the string is the number of characters it holds and length of a list is the number of elements it holds. And Zero indexing is supported in both.  
And also both(lists and strings) follow membership Operators.  
1) in: evaluates if the object on the left side is included in the object on the right side.
2) not in: evaluates if the object on the left side is not included in the object on the right side.


#### Slicing of List 
 1. The [:] notation represents the entire list, so list1[:] includes all elements of the list.
```python
print(list1[:] ) # output :['month', 'December', 3, 6.46, False]
```
2. using [:3] retrieves elements from the beginning up to (but not including) the element at index 3.
```python
print(list1[:3]) # output : ['month', 'December', 3]
```
3.list1[3:] retrieves elements starting from index 3 to the end of the list.
```python
print(list1[3:]) # output :[6.46, False]
```
4. Slicing with [1:4] includes elements from index 1 up to (but not including) index 4.
```python
print(list1[1:4]) # output :['December', 3, 6.46]
```
#### Membership Operators.
1. The in operator evaluates if an element exists within a string or list, returning True if it does.
```python
fruits = ['apple', 'banana', 'orange', 'grape', 'kiwi']
# Check if an element exists in a list
print('banana' in fruits)  # Output: True

# Check if an element does not exist in a list
print('watermelon' not in fruits)  # Output: True
```
2. The not in operator evaluates if an element does not exist within a string or list, returning True if it is not present.
```python
sentence = 'Python programming is fun and powerful'
# Check if a substring exists in a string
print('programming' in sentence)  # Output: True

# Check if a substring does not exist in a string
print('Java' not in sentence)  # Output: True
```
Strings are sequences of letters, while lists can be any type of object. The Main difference between strings and lists is strings are immutable while lists are mutable.  

Mutability: Lists are mutable (can be changed), while strings are immutable (cannot be changed after creation).  
Order is about whether the position of an element in the object can be used to access the element.
Order: Both strings and lists are ordered, meaning the position of an element can be used to access it. Both strings and Lists are ordered, which is why indexing works for them.  

#### Mutable Example: Lists
```python
shopping_list = ["apple", "banana", "cherry"]
shopping_list[1] = "orange"
print(shopping_list)
# Output: ["apple", "orange", "cherry"]

Example 2
numbers = [1, 2, 3, 4, 5]
original_id = id(numbers)  # Get the memory address of the original list
numbers[0] = 10
modified_id = id(numbers)  # Get the memory address after modification
print(original_id == modified_id)  # True (Same object)

```

#### Immutable Example: Strings
```python
greeting = "pay"
# The line below will result in an error
# greeting[0] = 'b'
# Error: 'str' object does not support item assignment

Example 2
greeting = "hello"
original_id = id(greeting)  # Get the memory address of the original string
# Concatenating to create a new string (seemingly modifying)
greeting += " world"
modified_id = id(greeting)  # Get the memory address after modification
print(original_id == modified_id)  # False (New object created)
```

# Creating a new string instead
```python
greeting = "bay"
print(greeting)
# Output: bay
```
### List Methods
1. len() returns how many elements are in a list.
```python
numbers = [1, 5, 2, 8, 3]
length = len(numbers)
print(f"Length of the list: {length}")
# Output: Length of the list: 5
```

2. max() returns the greatest element of the list. The maximum element in a list of numbers is the largest number.
```python
max_value = max(numbers)
print(f"Maximum value in the list: {max_value}")

# Output: Maximum value in the list: 8
```

3. min() returns the smallest element in a list. min is the opposite of max, which returns the largest element in a list.
```python
min_value = min(numbers)
print(f"Minimum value in the list: {min_value}")

# Output: Minimum value in the list: 1
```
4. sorted() returns a copy of a list in order from smallest to largest. Note that for string objects, sorted smallest to largest means sorting in alphabetical order.
```python
sorted_numbers = sorted(numbers)
print(f"Sorted list: {sorted_numbers}")

# Output: Sorted list: [1, 2, 3, 5, 8]
```
The max(), min(), and sorted() functions are undefined for lists that contain elements from different, incomparable types. It would raise a TypeError in such cases.


5. join() is a string method that takes a list of strings as an argument and returns a string consisting of the list elements joined by a separator string.
   
It is important to remember to separate each of the items in the list you are joining with a comma (,). Forgetting to do so will not trigger an error, but will also give you unexpected results.
```python
#Example1
new_str = ", ".join(["apple", "banana", "orange", "grape"])
print(new_str)

# Output: apple, banana, orange, grape

# Example 2
sentence = " ".join(["The", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog"])
print(sentence)

# Output: The quick brown fox jumps over the lazy dog
```

6. append() A helpful method called append adds an element to the end of a list.
```python
# Example
fruits = ['apple', 'banana', 'orange']
fruits.append('kiwi')
print(fruits)

# Output: ['apple', 'banana', 'orange', 'kiwi']
```
A data type is just a type that classifies data. This can include primitive (basic) data types like integers, booleans, and strings, as well as data structures, such as lists.

Data structures are containers that organize and group data types together in different ways. For example, some of the elements that a list can contain are integers, strings, and even other lists!

### Tuples
A tuple is a data structure in Python that is an immutable ordered sequence of elements, they are often used to store related pieces of information.  
 
1. Optional Parenthesis
In Python, you can define a tuple with or without parentheses. The parentheses are optional, and programmers often omit them if their presence doesn't improve code clarity. 
```python
# With Parentheses
coordinates_with_parentheses = (35.6895, 139.6917)
print(coordinates_with_parentheses)
print(type(coordinates_with_parentheses))
# output : (35.6895, 139.6917)
# output : <class 'tuple'>
# Without Parentheses (Optional)
coordinates_without_parentheses = 35.6895, 139.6917
print(coordinates_without_parentheses)
print(type(coordinates_without_parentheses))
# output:(35.6895, 139.6917)
# output: <class 'tuple'>
```
2. Tuple Unpacking 
Tuple unpacking allows you to assign the values of a tuple to multiple variables in a single line. In this example, the values (52, 40, 100) are unpacked into length, width, and height.
```python
# Tuple Unpacking Example
box_dimensions = 52,66, 95
length, width, height = box_dimensions
print("The dimensions are {} x {} x {}".format(length, width, height))
# output : The dimensions are 52 x 66 x 95
```
3. Immutable
Attempting to Change a Tuple (Results in an Error)
```python
coordinates = (35.6895, 139.6917)
# This line would raise an error
coordinates[0] = 40.7128
# output: 'tuple' object does not support item assignment
```
### Sets
A set is a mutable, unordered collection of unique elements. You can create a set from a list to quickly remove duplicates. 
1. creating a set
```python
# Creating a Set
numbers = [99, 100, 1, 3, 4, 99, 100]
unique_nums = set(numbers)
print(unique_nums)
# Output: {1, 3, 99, 100, 4}
```
2. The `in` operator checks if an element exists in the set.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
# Check for Element
print("mango" in fruits)  # Output: False
```
3. The `add` method adds a new element to the set.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
fruits.add("mango")
print(fruits)
# Output: {'grapefruit', 'orange', 'mango', 'banana', 'apple'}
```
4. The `remove` method removes a specific element from the set.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
fruits.remove("banana")
print(fruits)
# Output: {'grapefruit', 'orange', 'mango', 'apple'}
```
5. The `discard` method removes an element if it exists, but does not raise an error if it doesn't.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
fruits.discard("kiwi")
print(fruits)
# Output: {'grapefruit', 'orange', 'mango', 'apple'}
```
6. The pop() method in Python removes and returns an arbitrary (random) element from the set.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
print(fruits.pop())  # remove a random element
print(fruits)
# output :{"apple, "orange", "grapefruit"}
```
7. The `clear` method removes all elements, making the set empty.
```python
fruits = {"apple", "banana", "orange", "grapefruit"}
fruits.clear()
print(fruits)
# Output: set()
```
8. Set operations
Sets support mathematical operations like union, intersection, and difference, making them efficient for such operations.
```python
# Set Mathematical Operations
set1 = set(range(1000))
set2 = set(range(500, 1500))

# Union
union_set = set1.union(set2)

# Intersection
intersection_set = set1.intersection(set2)

# Difference
difference_set = set1.difference(set2)
```
 ### set operations are significantly faster than their list counterparts, especially for union, intersection, and difference operations.  
 

 ###  Dictionaries and Identity Operators
A dictionary is a mutable data type that stores mappings of unique keys to values. In Python, dictionaries use key-value pairs to organize data. Each key must be of an immutable type (e.g., strings, integers, or tuples), and keys within a dictionary do not have to share the same type.
1. Example
```python
# Creating a dictionary of countries and their capitals
countries_capitals = {"USA": "Washington, D.C.", "France": "Paris", "Japan": "Tokyo"}

# Accessing values using square brackets
print(countries_capitals["France"])  # Output: Paris

# Adding a new country and its capital to the dictionary
countries_capitals["Australia"] = "Canberra"

# Printing the updated dictionary
print(countries_capitals)
# output: {'USA': 'Washington, D.C.', 'France': 'Paris', 'Japan': 'Tokyo', 'Australia': 'Canberra'}
```
2. If you try to look up a key that is not in the dictionary using square brackets, it will raise a KeyError. To avoid this, you can use the get() method, which returns None (or a default value) if the key isn't found.
```python
print(countries_capitals.get("india"))     # Output: None
```
3. Checking if a key is in the dictionary
```python
print("india" in countries_capitals)        # Output: False
```
4. Identity Operators
Identity operators (is and is not) evaluate whether both sides have the same or different identities, respectively.
The is operator evaluates to True if both operands refer to the same object in memory. It checks for identity, meaning it checks if the objects are stored at the same memory address.
The is not operator evaluates to True if the operands do not refer to the same object in memory.
```python
countries_capitals = {"USA": "Washington, D.C.", "France": "Paris", "Japan": "Tokyo"}
n=countries_capitals.get("india")
print(n is None)      # Output: True (key not found, get returns None)
print(n is not None)  # Output: False (opposite of n is None)

```
5. Handling Absent Key with get():
get() allows specifying a default value to be returned if the key is not found:
```python
# Specifying a default value with get()
result_with_default = countries_capitals.get('Dubai', 'There\'s no such element!')
print(result_with_default)  # Output: "There's no such element!"
```
```python
# Creating a dictionary of student records
student_records = {
    'Alice': {
        'age': 22,
        'major': 'Chemistry',
        'grades': [90, 88, 92]
    },
    'Bob': {
        'age': 20,
        'major': 'Physics',
        'grades': [85, 89, 94]
    }
}

# Adding a new student
student_records['Charlie'] = {
    'age': 21,
    'major': 'Biology',
    'grades': [78, 92, 87]
}

# Adding a grade for an existing student
student_records['Alice']['grades'].append(95)

# Printing the updated dictionary
print(student_records)
# Output:
{
    'Alice': {
        'age': 22,
        'major': 'Chemistry',
        'grades': [90, 88, 92, 95]
    },
    'Bob': {
        'age': 20,
        'major': 'Physics',
        'grades': [85, 89, 94]
    },
    'Charlie': {
        'age': 21,
        'major': 'Biology',
        'grades': [78, 92, 87]
    }
}
```
### Control Flow
Control flow in Python refers to the order in which the lines of code are executed. It allows the programmer to dictate the execution flow based on certain conditions or loops.   

### if statement 
An if statement in Python is a conditional statement that allows you to control the flow of your code based on whether a given condition is true or false.
```python
# Check if the user's age is below 18
user_age = 20

if user_age < 18:
    print("Access denied. You must be 18 or older.")
else:
    print("Welcome! You have access to the content.")
# output: Welcome! You have access to the content.
```
#### How the if statement works
1. Keyword: An if statement starts with the keyword if, followed by the condition to be checked, in this case, user_age < 18.
  
2. Colon: The condition is followed by a colon: The colon signifies the beginning of a code block that will be executed if the condition is true.
  
3. Indented Block: The indented code block under the if statement is executed only if the condition is true. In the example, it prints a message denying access.
 
4. Else Block: Optionally, you can include an else block that contains code to be executed if the condition in the if statement is false. In this example, it prints a welcome message.

### if,elif, else
the if, elif (else if), and else statements are used to introduce decision-making logic into your code.
```python
# Check the weather and provide recommendations
weather = 'rainy'

if weather == 'sunny':
    print('Enjoy the sunshine!')
elif weather == 'rainy':
    print('Grab an umbrella!')
elif weather == 'snowy':
    print('Bundle up for the snow!')
else:
    print('Check the weather forecast for today.')
```
#### How If, Elif, Else Statements Work
1. if Statement: An if statement checks the first condition. If it is true, the code inside the corresponding block is executed, and the entire if-elif-else structure is exited.  
2. elif Statement: If the condition in the if statement is false, the next elif (else if) statement is checked. If its condition is true, the code inside the corresponding block is executed, and the structure is exited.
3. else Statement: If none of the conditions in the if and elif statements are true, the else statement is executed. The else block is optional and provides a default action if no other conditions are met.
4. Colon and Indentation: Like with the if statement, each elif and else statement ends with a colon: and is followed by an indented block of code. The indentation is crucial in Python to define the scope of the code blocks.

### Boolean Expressions for conditions
```python
# Evaluate weather conditions
is_raining = True
is_sunny = False

if is_raining and is_sunny:
    print("Is there a rainbow?")
elif is_raining and not is_sunny:
    print("It's just raining.")
elif not is_raining and is_sunny:
    print("Enjoy the sunshine!")
else:
    print("No rain or sunshine today.")
```
1. Avoid using True or False as conditions
```python
# Bad Example 1
if True:
    print("This indented code will always get run.")

# Bad Example 2
if is_cold or not is_cold:
    print("This indented code will always get run.")
```
2. Carefully use logical operators
```python
# Bad Example
if weather == "snow" or "rain":
    print("Wear boots!")
```
3. Don't compare a boolean variable with == True or == False
```python
# Bad Example
if is_cold == True:
    print("The weather is cold.")

# Good Example
if is_cold:
    print("The weather is cold.")
```
4. For checking if a boolean is False, use the not operator
```python
if not is_warm:
    print("The weather is not warm.")
```
### Truth value testing
In Python, when using a non-boolean object as a condition in an if statement, Python checks for its truth value to determine whether or not to execute the indented code. By default, the truth value of an object in Python is considered True unless specified as False in the documentation.

Here are some built-in objects in Python that are considered False:

1. Constants defined to be false: None and False
2. Zero of any numeric type: 0, 0.0, 0j, Decimal(0), Fraction(0, 1)
3. Empty sequences and collections: "", (), [], {}, set(), range(0)
```python
# Using truth value testing with a non-boolean object
unread_messages = 0

# Check the truth value of unread_messages
if not unread_messages:
    print("You have no unread messages.")
else:
    print("You have unread messages.")
# Output and explanation: In this example, the variable unread_messages is assigned the value 0, which is considered False in a truth value test. Therefore, the indented code inside the if block is executed, printing "You have no unread messages."
```
### For and While Loops
An object that can return one of its elements at a time. This can include sequence types, such as strings, lists, and tuples, as well as non-sequence types, such as dictionaries and files.

```python
ipl_teams = ["csk", "rr", "rcb"]
for teams in ipl_teams:
  print(teams)
# output:
csk
rr
rcb
```
#### Components of a for Loop
1. Loop Header:
Starts with the for keyword.
Specifies the iteration variable (teams) and the iterable (ipl_teams).
Ends with a colon :.
2. Loop Body:
Indented block of code executed in each iteration.
3. Iteration Process:
The iteration variable takes the value of the next element in the iterable (ipl_teams).
The loop continues until all elements in the iterable have been processed.
4. Output:

#### Using range() Function with for Loops  
range(start=0, stop, step=1)  
start: The first number of the sequence (default is 0).  
stop: One more than the last number of the sequence (must be specified).  
step: The difference between each number in the sequence (default is 1).  

```python
for i in range(3):
    print(f"Hello, iteration {i + 1}!")
# output:
Hello, iteration 1!
Hello, iteration 2!
Hello, iteration 3!
```
#### creating a new list
```python
ipl_teams = ['csk','rr', 'rcb', 'mi']
capitalized_teamss = []

for teams in ipl_teams:
    capitalized_teamss.append(teams.title())
print(capitalized_teams)
# output :['Csk', 'Rr', 'Rcb', 'Mi']
```

#### Modifying a list in place
```python
teams = ['csk','rr', 'rcb', 'mi']
for index in range(len(teams)):
    teams[index] = teams[index].title()
print(teams)
# output : ['Csk', 'Rr', 'Rcb', 'Mi']
```
### Building Dictionaries
1. Using the iteration by for loop
```python
# Method 1: Using a for loop
animals = ['dog', 'cat', 'dog', 'fish', 'cat', 'bird', 'dog', 'fish', 'bird', 'cat']
animal_counter = {}

# Iterate through each animal in the list
for animal in animals:
    # Check if the animal is already a key in the dictionary
    if animal in animal_counter:
        # If yes, increment the existing count by 1
        animal_counter[animal] += 1
    else:
        # If no, add the animal to the dictionary with a count of 1
        animal_counter[animal] = 1

# Print the final animal count dictionary
print("Animal Count (Method 1):", animal_counter)
# output: Animal Count (Method 1): {'dog': 3, 'cat': 3, 'fish': 2, 'bird': 2}
```
2. Using the get() method

 word_counter[word] = word_counter.get(word,0) + 1, since the key 'apple' doesn't yet exist in the dictionary, get() will return the value 0 and word_counter[word] will be set to 1.

Once it encounters a word that already exists in word_counter, the value for that key is incremented by 1. On the second appearance of 'the', the key's value would add 1 again, resulting in 2.
```python
# Method 2: Using the get method
fruits = ['apple', 'orange', 'banana', 'apple', 'banana', 'orange', 'kiwi', 'apple', 'kiwi', 'orange']
fruit_counter = {}

# Iterate through each fruit in the list
for fruit in fruits:
    # Use the get method to fetch the current count or default to 0
    fruit_counter[fruit] = fruit_counter.get(fruit, 0) + 1

# Print the final fruit count dictionary
print("Fruit Count (Method 2):", fruit_counter)
# output: Fruit Count (Method 2): {'apple': 3, 'orange': 3, 'banana': 2, 'kiwi': 2}
```
### Iterating through Dictionaries 
When you iterate through a dictionary using a for loop, doing it the normal way, like   

for n in some_dict, will only give you access to the keys in the dictionary - which is what you'd want in some situations.  
```python
animals = {'dog': 3, 'cat': 3, 'fish': 2, 'bird': 2}
for key in animals:
 print(key)
# output: dog
         cat
         fish
         bird
```
If we wish to iterate through both keys and values, you can use the built-in method items like this:
```python
for key, value in animals.items():
    print("Animal:{},count: {}".format(key, value))
# output : Animal: dog, count: 3
           Animal: cat, count: 3
           Animal: fish, count: 2
           Animal: bird, count: 2
```
### While loops
1. The first line starts with the while keyword, indicating this is a while loop.
2. Following that is a condition to be checked. In this example, that's counter <= 5.
3. The while loop heading always ends with a colon:
4. Indented after this heading is the body of the while loop. If the condition for the while loop is true, the code lines in the loop's body will be executed.
5. We then go back to the while heading line, and the condition is evaluated again. This process of checking the condition and then executing the loop repeats until the condition becomes false.
6. When the condition becomes false, we move on to the line following the body of the loop, which will be unindented.
```python
# Initialize a counter
counter = 1

# Define the condition for the while loop
while counter <= 5:
    print(counter)
    counter += 1  # Increment the counter

# Output:
# 1
# 2
# 3
# 4
# 5
```
The indented body of the loop should modify at least one variable in the test condition. If the value of the test condition never changes, the result is an infinite loop!

### Zip and Enumerate
Zip returns an iterator that combines multiple iterables into one sequence of tuples.each tuple contains the elements in that position from all the iterables.
1. Zipping 
```python
ranks = [1,2,3]
persons = ["arjun","krishna","ram"]
for rank,person in zip(ranks,persons):
 print("{}: {}".format(rank,person))
# output : 1: arjun
           2: krishna
           3: ram
```
2. unzipping - using an asterisk, we can unzip a list into tuples.
```python
rank_list = [('arjun', 1), ('krishna', 2), ('ram', 3)]
ranks, persons = zip(*rank_list)
print(ranks)
print(persons)
print(type(ranks))
# output :
('arjun', 'krishna', 'ram')
(1, 2, 3)
<class 'tuple'>
```
3. Enumerate
enumerate is a built-in function that returns an iterator of tuples containing  indices and values of a list.
```python
rank_list = [('arjun', 1), ('krishna', 2), ('ram', 3)]
for rank in enumerate(rank_list):
    print(rank)
# output : (0, ('arjun', 1))
           (1, ('krishna', 2))
           (2, ('ram', 3))
The output is of type tuple
```
### List Comprehensions

### Functions
Functions are useful chunks of code that allow you to encapsulate a task.
Encapsulation is a task to carry out a whole series of steps with one single command.
#### Defining functions
Arguments are the values passed in as inputs to a function.  
print provides output to the console while return provides the value that you can store and work with code later  
The function header always starts with the def keyword, which indicates that this is a function definition.  
Then comes the function name (here, bmi), which follows the same naming conventions as variables.  
Immediately after the name are parentheses that may include arguments separated by commas (here, mass and heights). Arguments, or parameters, are values that are passed in as inputs when the function is called, and are used in the function body. If a function doesn't take arguments, these parentheses are left empty.  
The header always ends with a colon:  
```python
# Body Mass Index (BMI) is a person's weight in kilograms (or pounds) divided by the square of height in meters (or feet)
def bmi(mass,height):
 x = mass/height
 return x

# We will perform function call
print(bmi(65,1.5))
# output: 43.333336
```
#### Function Body
The rest of the function is contained in the body, which is where the function does its work.  
The body of a function is the code indented after the header line. Here, the two lines assign x and return the x= mass/height.  
Within this body, we can refer to the argument variables and define new variables, which can only be used within these indented lines.  
The body will often include a return statement, which is used to send back an output value from the function to the statement that called the function. A return statement consists of the return keyword followed by an expression evaluated to get the output value for the function. If there is no return statement, the function simply returns None.


#### Naming Conventions for Functions
Function names follow the same naming conventions as variables.  
Only use ordinary letters, numbers and underscores in your function names. They can’t have spaces and need to start with a letter or underscore.  
You can’t use reserved words or built-in identifiers that have important purposes in Python, which you’ll learn about throughout this course.

#### default arguments
We can add default arguments in a function to have default values for parameters that are unspecified in a function call.  
Here height is to 1.7,if that parameter is omitted in a function call. If we call bmi(65), the function will use 65 as mass and 1.7 as the height. However, if we call bmi(65,1.5) the 1.5 will simply overwrite the default value of 1.7.  
```python
def bmi(mass,height=1.7):
 x = mass/height
 return x

# We will perform function call
print(bmi(65,1.5))
# output: 43.333336
```
Also notice here we are passing values to our arguments by position. It is possible to pass values in two ways - by position and by name. Each of these function calls are evaluated the same way.  
```python
bmi(65, 1.5)  # pass in arguments by position
bmi(mass=65,height=1.5)# pass in arguments by name
```
### Variable scope
Variable scope refers to which parts of a program a variable can be referenced, or used, from. 
It's important to consider scope when using variables in functions. If a variable is created inside a function, it can only be used within that function. Accessing it outside that function is not possible.  
Variables defined outside functions,is said to have a global scope.  
we can still access the value of the global variable `word` within this function. However, the value of a global variable can not be __modified__ inside the function. If you want to modify that variable's value inside this function, it should be passed in as an argument.  


### Doc string
A type of comment used to explain the purpose of function and how it should be used. Docstrings are surrounded by triple quotes. 

### Lamda expressions
we can use lambda expression to create an anonymous function. That is these functions do not have a name.  
Components of a Lambda Function
1. The lambda keyword is used to indicate that this is a lambda expression.  
2. Following lambda are one or more arguments for the anonymous function separated by commas, followed by a colon :. Similar to functions, the way the arguments are named in a lambda expression is arbitrary.
3. Last is an expression evaluated and returned in this function. This is much like an expression you might see as a return statement in a function.  
4. With this structure, lambda expressions aren’t ideal for complex functions but can be very useful for short, simple functions.  

With a lambda expression, this function:
```python
def multiply(x, y):
    return x * y
```
can be reduced to:
```python
multiply = lambda x, y: x * y
```
Both of these functions are used in the same way. In either case, we can call multiply like this:
```python
multiply(4, 7)
```
This returns 28.


### scripting


### Errors and Exceptions
1. Syntax errors occur when Python can’t interpret our code since we didn’t follow the correct syntax for Python. These are errors you’re likely to get when you make a typo, or you’re first starting to learn Python.

2. Exceptions occur when unexpected things happen during the execution of a program, even if the code is syntactically correct. There are different types of built-in exceptions in Python, and you can see which exception is thrown in the error message.

### Exception handling
1. Try Statement: We can use try statements to handle exceptions. There are four clauses you can use (one more in addition to those shown in the video).
2. try: This is the only mandatory clause in a try statement. The code in this block is the first thing that Python runs in a try statement.
3. except: If Python runs into an exception while running the try block, it will jump to the except block that handles that exception.
4. else: If Python runs into no exceptions while running the try block, it will run the code in this block after running the try block.
5. finally: Before Python leaves this try statement, it will run the code in this block under any conditions, even if it's ending the program. E.g., if Python ran into an error while running code in the except or else block, this finally block will still be executed before stopping the program.
#### specifying exceptions
We can actually specify which error we want to handle in an except block like this:
```python
try:
    # some code
except ValueError:
    # some code
```
Now, it catches the ValueError exception, but not other exceptions. If we want this handler to address more than one type of exception, we can include a parenthesized tuple after the except with the exceptions.
```python
try:
    # some code
except (ValueError, KeyboardInterrupt):
    # some code
```
Or, if we want to execute different blocks of code depending on the exception, you can have multiple except blocks.
```python
try:
    # some code
except ValueError:
    # some code
except KeyboardInterrupt:
    # some code
```
