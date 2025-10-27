# _Python_

_Python is a programming language created in the early 1990s by **Guido van Rossum**._

_From the beginning, the idea behind the language was to make programming simpler, more intuitive, and closer to natural thought._
_The simplicity is one of the main reasons Python is loved by beginners, but behind its friendly surface lies incredible power, which is why professionals use it for:_

- :globe_with_meridians: _**Large-Scale Applications**_
- :electron: _**Data Science**_
- :brain: _**Artificial Intelligence**_
- :robot: _**Robotics**_

_The guiding principles of Python's design are encapsulated in the **Zen of Python**, a short manifesto that emphasizes simplicity, explicitness, and elegance. These principles are not abstract ideals but practical guidelines that shape the language itself._

## _Overview_

_Python is a **high-level**, **interpreted language**, designed to prioritize readability and clarity. Its source code is automatically compiled into **bytecode** (an intermediate, low-level representation of the program), which is then executed by the interpreter, enabling rapid testing and development._

_<sub>In Python everything is an object, and every object has a type.<sub>_

_Another defining aspect of Python is its **dynamic typing system**. Variables do not need to be declared with explicit types; the type is inferred automatically at runtime. At the same time, Python maintains strong rules for type behavior, ensuring that values behave predictably even in the absence of explicit declarations._

_The language does not confine developers to a single paradigm. **Procedural programming**, **Object-Oriented design**, and **Functional constructs** can coexist within the same project. This versatility allows Python to adapt to a wide variety of domains, from small scripts that automate routine tasks to large systems that require complex architectures._

_Python is also **platform-independent**, working consistently across Windows, macOS, and Linux environments. This portability simplifies deployment and collaboration, ensuring that code developed in one context can easily be executed in another. The **open-source** nature of the language has cultivated an exceptionally large and active community, which contributes documentation, tutorials, and improvements to the ecosystem._

_A significant advantage of Python lies in its comprehensive **standard library**. Modules for mathematics, file manipulation, networking, and system interaction are included with every installation. Beyond this foundation, the **Python Package index** provides access to thousands of external libraries, extending the language into specialized fields._

## _Syntax Information_

_The syntax of Python distinguishes it from many other languages. **Indentation** is used to define the structure of code, replacing the braces or keywords that are common elsewhere. The result is source code that is clean, uniform, and immediately comprehensible._\

_It is also **case-sensitive**, meaning that identifiers with different letter cases are treated as distinct names (**keywords** are fixed in lowercase)._

_In Python, comments allow programmers to include explanatory notes that are ignored during execution. We can insert two types of comments into the code :_

* _```single-line comment``` : begins with the characters ```#```_
* _```multi-line comment``` : starts and ends with the sequence ```"""``` or ```'''```_

_Python allows a single statement to span multiple lines for readability. This can be done using a **backslash** (```\```) at the end of a line, indicating that the statement continues on the next line._
_Alternatively, enclosing expressions in **parentheses** allows Python to automatically treat multiple lines as a single statement without a backslash._

## _Variables and Data Types_

_A variable in Python is a symbolic name that stores data in memory. Variables act as containers for values, allowing programs to work with data in a flexible way. In Python, variables are created the moment a value is assigned to them (there is no need to declare their type explicitly)._

_```name = "Chris"```_\
_```age = 25```_

_<sub>**name** stores a string<sub>_\
_<sub>**age** stores an integer<sub>_

_Python does not have true constants; however, by convention, variables intended to remain unchanged are written in uppercase letters, signaling to programmers that they should not be modified._

_In Python, every value and variable belongs to a **data type**, which determines how the data is stored, how it can be manipulated, and what operations can be performed on it. Python orgranizes data types into two broad categories: **built-in types** and **user-defined types**._

_<sub>The ```type()``` function is the built-in way to check the type of any value or variable. It returns the class of the object being inspected.<sub>_

### _Built-in Types_

_Python provides a set of built-in types that are always available without importing additional modules. These types form the core foundation of the language and are designed to handle most everyday programming needs._\

#### _Primitive Built-in Types_

_These are the simplest types, representing single pieces of data:_

* _**Integers** (```int```): whole numbers without decimal points (they can be positive, negative, or zero). Python supports integers of arbitrary size, limited only by available memory._

  ```x = 42```
  
* _**Floating-point numbers** (```float```): numbers that contain decimal points._

    ```x = 3.42```

* _**Strings** (```str```): ordered sequences of characters enclosed in quotes (they can contain letters, numbers, symbols, and whitespace). Strings are **immutable**, meaning they cannot be changed after creation, though new strings can be generated from them._

    ```name = "Chris"```

* _**Booleans** (```bool```): Booleans represent truth values (```True``` or ```False```)._

    ```condition = True```

* _**NoneType** (```None```): special type representing the absence of a value or a null value._

    ```result = None```

#### _Composite Built-in Types_

_These store multiple values in a structured way:_

* _**Lists** (```list```): **ordered** collections that can store items of different types. They are **mutable**, meaning items can be changed, added, or removed. List are versatile for storing sequences of data._

    ```numbers = [1, 2, 3, 4]```

* _**Tuples** (```tuple```): **ordered** collections like lists, but **immutable**. They are often used to group related data and can seerve as keys in dictionaries._

    ```point = (42, 24)```

* _**Sets** (```set```): **unordered** collections of unique elements. They are useful for eliminating duplicates and performing mathematical set operations._

    ```unique_numbers = {1, 2, 3}```

* _**Dictionaries** (```dict```): dictionaries store data in **key-value pairs**. They are **mutable**, **unordered**, and highly efficient for lookups. Keys must be unique and immutable._

    ```person = {"name" : "Chris", "age" : 29}```

#### _Special Built-in Types_

_Python includes additional specialized types for particular needs:_

* _**Bytes** (```bytes```) and **Bytearrays** (```bytearray```) for binary data._
* _**Range** (```range```) for sequences of numbers._
* _**Complex Numbers** (```complex```) for mathematical computations involving imaginary numbers._
* _**Frozen Sets** (```frozenset```) which are immutable sets._

### _User-defined Data Types_

_Python allows creation of custom data types to represent more complex or specific structures. User-defined types are typically created using:_

* _**Classes**: define the structure and behavior of objects in **object-oriented programming**._
* _**Functions returning custom structures**._
* _**Modules containing user-created types or constants**._

```class Person:```\
```  def __init__(self, name, age):```\
```    self.name = name```\
```    self.age = age```

_<sub>The example shows a simple user-defined type using a class. This creates a new type ```Person``` with attributes ```name``` and ```age```.<sub>_

## _Operators and Expressions_

_An operator in Python is a symbol or keyword that performs a specific action on one or more values (known as **operands**)._\
_When operators are combined with values, the result is an **expression**. Expressions are the core of computation in Python (every calculation, comparison, or logical decision rests on them)._

### _Arithmetic Operators_

_Arithmetic operators perform basic mathematical operations. They apply to numeric types such as integers, floats, and even complex numbers._

* _**Addition**: ```+```_

  _<sub>The arithmetic operator ```+``` can also be applied to strings, allowing **concatenation**, combining two strings into a single new string.<sub>_
  
* _**Subtraction**: ```-```_
* _**Multiplication**: ```*```_

  _<sub>The arithmetic operator ```*``` can also be applied to strings, allowing **repetition**, creating multiple copies of a string in sequence.<sub>_

* _**Division**: ```/``` (always returns a float, even when dividing integers)_
* _**Floor Division**: ```//``` (returns the integer quotient, discarding the remainder)_
* _**Modulo**: ```%``` (returns the remainder of a division)_
* _**Exponentiation**: ```**``` (raises a number to the power of another)_

_<sub>Python allows arithmetic operations to be written in a more compact form using **augmented assignment operators**. For example instead of writing ```a = a + 1```, the same effect can be achieved with ```a += 1```.<sub>_

### _Comparison Operators_

_Comparison operators evaluate the relationship betweeen values and return Boolean results. They are crucial for decision-making in programs._

* _**Equal**: ```==```_
* _**Not Equal**: ```!=```_
* _**Greater than**: ```>```_
* _**Less than**: ```<```_
* _**Greater than or Equal to**: ```>=```_
* _**Less than or Equal to**: ```<=```_

### _Logical Operators_

_Logical operators combine Boolean values to form more complex conditions._

* _```and```: returns True if both operands are True._
* _```or```: returns True if at least one operand is True._
* _```not```: negates the truth value._

### _Assignment Operators_

_The assignment operator ```=``` places a value into a variable. In addition, Python supports **augmented assignment**, which combines an operation with assignment, simplifying expressions._

_<sub>```x += 5``` is equivalent to ```x = x + 5```<sub>_

### _Membership Operators_

_Membership operators test whether a value is present in a sequence such as a list, string, or tuple._

* _```in```: returns True if the element is present._
* _```not in```: returns True if the element is absent._

```fruits = ["apple", "cherry", "mango"]```\
```print("apple" in fruits)```  --> True\
```print("grape" not in fruits``` --> True

### _Identity Operators_

_Identity operators check whether two variables refer to the same object in memory, not just whether they contain the same value._

* _```is```: returns True if both variables point to the same object._
* _```is not```: returns True if they point to different objects._

```a = [1, 2, 3]```\
```b = a```\
```c = [1, 2, 3]```\

```print(a is b)``` --> True (same object)\
```print(a is c)``` --> False (different objects, same content)

### _Operator Precedence_

_When multiple operators appear in an expression, Python follows a strict order of evaluation known as operator precedence. For instance, multiplication and division are performed before addition and subtraction, just like in standard arithmetic._\
_Parentheses can always be used to override precedence and make intentions explicit._

## _Type Conversion_

_In Python, values often need to be transformed from one type into another. This process is known as **type conversion** or **type casting**. It allows data to be adapted to the requirements of a particular operation or context._\
_Two primary forms of conversion exist: **implicit conversion** and **explicit conversion**._

### _Implicit Conversion_






## _Escape Sequences and Output Formatting_

_In Python, strings can contain special characters that cannot be typed or displayed directly._
_These characters are represented using **escape sequences**, which begin with a backslash (```\```). Escape sequences allow programmers to include formatting commands, quotation marks, or special symbol within strings, making text more expressive and structured._
_Common escape sequences include :_

* _```\n``` : inserts a **newline**, moving the cursor to the next line._
* _```\t``` : inserts a **horizontal tab**, useful for aligning text._
* _```\\``` : inserts a literal backslash._
* _```\'``` and ```\*``` : include single or double quotes inside a string without ending it._

_In Python, formatting output is essential when displaying data in a clear and structured way._
_While simple concatenation or printing can work for short messages, more complex programs often require **aligned columns**, **fixed widths**, or **controlled decimal precision**. Python provides several methods to achieve this :_

#### _F-strings_

_F-strings are string literals prefixed with ```f``` or ```F```, in which expressions inside ```{}``` are evaluated and inserted directly into the string. Format specifiers can follow a colon (```:```) inside the braces._
_Common specifiers :_

* _**Alignment** : ```<``` left align, ```^``` center align, ```>``` right-align._
* _**Width** : a number specifying the minimum width of the field._
* _**Precision** : for floats, ```.nf``` sets ```n``` decimal places._

  _```name = "Chris"```_\
  _```age = 25```_\
  _```height = 1.753```_

  _```print(f"{'Name':<10} | {'Age':^5} | {'Height':>7}")```_

    _<sub>Print header with aligned columns<sub>_
  
  _```print(f"{name:<10} | {age:^5} | {height:>7.2f}")```_

    _<sub>Print data row with formatting<sub>_

#### _format() Method_

_The ```format()``` method works similarly but separates the string template from the values. Placeholders ```{}``` in the string are replaced by arguments passed to ```format()```._

  _```print("{:<10} | {:^5} | {:>7.2f}".format(name, age, height))```_

#### _Old-Style % Operator_

_This older style uses **format codes** that indicate type and optional width/precision :_

* _```%s``` : **string**_
* _```%d``` : **integer**_
* _```%f``` : **floating-point number**_

_Width and precision are added after ```%``` :_

_```print("%-10s | %5d | %7.2f" % (name, age, height))```_

## _Basic String Methods_

_Strings in Python are objects just like everything else. They come with a variety of **built-in methods** that simplify common operations. These methods allow programmers to manipulate, format, and inspect strings efficiently, without having to write complex code from scratch._
_Among the most frequently used string methods are :_

* _```.upper()``` : convert all characters in a string to uppercase._
* _```.lower()``` : convert all characters in a string to lowercase._
* _```.strip()``` : removes any leading and trailing whitespace (or specified characters) from a string._

  _```text = "  Hello World    "```_\
  _```print(text.strip())``` result = "Hello World"_

* _```.replace(old, new)``` : returns a new string where occurrences of **old** are replaced with **new**_

  _```text = "I like apples"```_\
  _```print(text.replace("apples", "oranges"))``` result = "I like oranges"_

* _```.split(separator)``` : splits a string into a list of substrings based on the specified separator (default is any whitespace)._

  _```text = "Python is fun"```_\
  _```words = text.split()```_\
  _```print(words)``` result = ["Python", "is", "fun"]_

* _```.join(iterable)``` : concatenates elements from an iterable (like a list of strings) into a single string, with the original string acting as a separator._

  _```words = ["Python", "is", "fun"]```_\
  _```sentence = " ".join(words)```_\
  _```print(sentence)``` result = "Python is fun"_

* _```.find(substring)``` : returns the index of the first occurrence of **substring** in the string or **-1** if not found._
* _```.startswith(prefix)``` : check whether the string begins with the specified substring, returning **True** or **False**._
* _```.endswith(suffix)``` : check whether the string ends with the specified substring, returning **True** or **False**._

## Built-in Functions

_Python provides a large collection of **built-in functions** that are always available without importing additional modules. These functions perform common operations on data, allowin programmers to write concise and readable code without reinventing basic functionality. Built-in functions work across data types, depending on the operation, and often simplify complex tasks into single function calls._

_The most frequently used functions are :_

* _```abs()``` : returns the absolute value of a number, effectively removing any negative sign._

  _```print(abs(-7))``` result = 7_
  
* _```round()``` : rounds a floating-point number to the nearest integer, or to a specified number of decimal places._

  _```print(round(3.14159, 2))``` result = 3.14_

* _```len()``` : returns the number of items in a sequence, such as a string, list or tuple._
* _```type()``` : returns the type of a value or variable, providing insight into how Python classifies the data._
* _```max()``` : returns the largest value from a sequence or a set of arguments._

  _```numbers = [4,7,1,9]```_\
  _```print(max(numbers))``` result = 9_

* _```min()``` : returns the smallest value from a sequence or a set of arguments._

  _```numbers = [4, 7, 1, 9]```_\
  _```print(min(numbers))``` result = 1_

* _```sum()``` : calculates the total of all numeric elements in a sequence._
* _```sorted()``` : returns a new list containing all items from a sequence in ascending order (or descending if specified)._

  _```numbers = [4, 2, 9, 1]```_\
  _```print(sorted(numbers))``` result = [1, 2, 4, 9]_\
  _```print(sorted(numbers, reverse = True))``` result = [9, 4, 2, 1]_

* _```input()``` : allows the program to receive input from the user as a string._
