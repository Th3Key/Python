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

#### _Arithmetic Operators_

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

#### _Comparison Operators_

_Comparison operators evaluate the relationship betweeen values and return Boolean results. They are crucial for decision-making in programs._

* _**Equal**: ```==```_
* _**Not Equal**: ```!=```_
* _**Greater than**: ```>```_
* _**Less than**: ```<```_
* _**Greater than or Equal to**: ```>=```_
* _**Less than or Equal to**: ```<=```_

#### _Logical Operators_

_Logical operators combine Boolean values to form more complex conditions._

* _```and```: returns True if both operands are True._
* _```or```: returns True if at least one operand is True._
* _```not```: negates the truth value._

#### _Assignment Operators_

_The assignment operator ```=``` places a value into a variable. In addition, Python supports **augmented assignment**, which combines an operation with assignment, simplifying expressions._

_<sub>```x += 5``` is equivalent to ```x = x + 5```<sub>_

#### _Membership Operators_

_Membership operators test whether a value is present in a sequence such as a list, string, or tuple._

* _```in```: returns True if the element is present._
* _```not in```: returns True if the element is absent._

```fruits = ["apple", "cherry", "mango"]```\
```print("apple" in fruits)```  --> True\
```print("grape" not in fruits``` --> True

#### _Identity Operators_

_Identity operators check whether two variables refer to the same object in memory, not just whether they contain the same value._

* _```is```: returns True if both variables point to the same object._
* _```is not```: returns True if they point to different objects._

```a = [1, 2, 3]```\
```b = a```\
```c = [1, 2, 3]```\

```print(a is b)``` --> True (same object)\
```print(a is c)``` --> False (different objects, same content)

#### _Operator Precedence_

_When multiple operators appear in an expression, Python follows a strict order of evaluation known as operator precedence. For instance, multiplication and division are performed before addition and subtraction, just like in standard arithmetic._\
_Parentheses can always be used to override precedence and make intentions explicit._

## _Type Conversion_

_In Python, values often need to be transformed from one type into another. This process is known as **type conversion** or **type casting**. It allows data to be adapted to the requirements of a particular operation or context._\
_Two primary forms of conversion exist: **implicit conversion** and **explicit conversion**._

### _Implicit Conversion_

_Implicit conversion, also known as **type coercion**, is the process by which Python automatically converts one data type into another during an operation. This behavior ensures that computations between different types can proceed without raising errors._
_When two operands of different types appear in an expression, Python promotes the smaller or less complex type to the more general one in order to preserve information. For example, when an integer and a floating-point number are combined, the integer is automatically converted into a float before the operation is executed._

_```x = 10``` int_\
_```y = 2.5``` float_\
_```result = x + y``` int is converted to float_\ 
_```print(result)``` result = 12.5_\
_```print(type(result))``` output = <class 'float'>_

_Python performs this silently and safely, ensuring that no data is lost. Implicit conversion most often occurs among **numeric types**, while conversions involving incompatible types require explicit intervention._

### _Explicit Conversion_

_Explicit conversion, also known as **type casting**, occurs when the programmer intentionally transforms a value from one type to another using built-in functions. This approach offers full control over how data is inerpreted and ensures that conversions happen only when intended._
_The most common conversion functions are :_

* _```int()``` : converts a value into an integer (truncates decimals if presents)_
* _```float()``` : converts a value into a floating-point number_
* _```str()``` : converts a value into a string representation_
* _```bool()``` : converts a value into a Boolean (non-zero or non-empty values become ```True```)_

_```x = 3.8```_\
_```y = int(x)``` y = 3_\
_```z = str(y)``` z = "3"_

_Explicit conversion is essential when working with user input, file data, or mixed-type operations, as it ensures that values are processed correctly according to the program's logic._

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

## Built-in Functions

_Python provides a large collection of **built-in functions** that are always available without importing additional modules. These functions perform common operations on data, allowin programmers to write concise and readable code without reinventing basic functionality. Built-in functions work across data types, depending on the operation, and often simplify complex tasks into single function calls._

_The most frequently used functions are :_

* _```print()``` : outputs information to the standard console, allowing programmers to display messages, variable values, or results of operations._

  _```print("Hello World!")```_

  _The function can take multiple arguments, separated by commas, and automatically inserts a space between them._

  _```print("Hello", "World")```_

  _By default it ends with a newline character (```\n```), but this behavior can be customized using the ```end``` parameter._

  _```print("Hello", "World", end = "!")``` outputs : Hello World!_

  _<sub>By default it is ```end = "\n"```.<sub>_

* _```input()``` : allows the program to receive input from the user as a string._
* _```len()``` : returns the number of items in a sequence, such as a string, list or tuple._
* _```type()``` : returns the type of a value or variable, providing insight into how Python classifies the data._
* _```sum()``` : calculates the total of all numeric elements in a sequence._
* _```abs()``` : returns the absolute value of a number, effectively removing any negative sign._

  _```print(abs(-7))``` result = 7_
  
* _```round()``` : rounds a floating-point number to the nearest integer, or to a specified number of decimal places._

  _```print(round(3.14159, 2))``` result = 3.14_

* _```max()``` : returns the largest value from a sequence or a set of arguments._

  _```numbers = [4,7,1,9]```_\
  _```print(max(numbers))``` result = 9_

* _```min()``` : returns the smallest value from a sequence or a set of arguments._

  _```numbers = [4, 7, 1, 9]```_\
  _```print(min(numbers))``` result = 1_

* _```sorted()``` : returns a new list containing all items from a sequence in ascending order (or descending if specified)._

  _```numbers = [4, 2, 9, 1]```_\
  _```print(sorted(numbers))``` result = [1, 2, 4, 9]_\
  _```print(sorted(numbers, reverse = True))``` result = [9, 4, 2, 1]_

## _Basic String Methods_

_Strings in Python are objects just like everything else. They come with a variety of **built-in methods** that simplify common operations. These methods allow programmers to manipulate, format, and inspect strings efficiently, without having to write complex code from scratch._
_Among the most frequently used string methods are :_

* _```.isalnum()``` : returns ```True``` if all characters in the string are **alphanumeric** (letters or digits) and there is at least one character._

  _<sub>Does not allow whitespace (or punctuation)<sub>_

* _```.isalpha()``` : returns ```True``` if all characters are ```alphabetic``` and the string contains at least one character._
* _```.isdigit()``` : returns ```True``` if the string contains only digits._
* _```islower()``` : returns ```True``` if all alphabetic characters are lowercase._
* _```isupper()``` : returns ```True``` if all alphabetic characters are uppercase._
* _```isspace()``` : returns ```True``` if the string contains only whitespace characters (spaces, tabs, or newlines)._
* _```istitle()``` : returns ```True``` if the string follows the rules of title case (the first letter of each word is uppercase)._
* _```.upper()``` : convert all characters in a string to uppercase._
* _```.lower()``` : convert all characters in a string to lowercase._
* _```.strip()``` : removes any leading and trailing whitespace (or specified characters) from a string._

  _```text = "  Hello World    "```_\
  _```print(text.strip())``` result = "Hello World"_

* _```.replace(old, new)``` : returns a new string where occurrences of **old** are replaced with **new**._

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

## _Input and Output Redirection_

_In Python, standard input and output are normally connected to the keyboard and the screen. When a program calls ```input()```, data is read from the keyboard, and when ```print()``` is used, the result is displayed on the screen._
_However, in many situations, it is useful to **redirect** these streams, meaning that the source of destination of input and output can be changed. This process is known as **input/output redirection**._

_For example, the output of a program can be sent to a file instead of the screen, or input can be taken from a file rather than typed manually. This allows automation, data logging, or interaction with other programs._

_In most cases, redirection is handled at the **operating system level**, using commands in the terminal or shell._

* _```python program.py > output.txt``` : redirects standard output to a file (if the file **does not exist**, it will be **automatically created**, if the file **already exists**, it will be **overwritten**)_
* _```python program.py < input.txt``` : redirects standard input from a file (the file must already exist because the program expects to read data from it, if the file is missing, an error will occur)_
* _```python program.py >> output.txt``` : appends output to an existing file (if the file **does not exist**, it will be **automatically created**, if the file **already exists**, the new output will be **added** to the end of the existing content)_

_Whithin Python itself, similar behavior can be achieved programmatically by opening files and reassigning the standard streams._

... TO FINISH ...

## _Control Flow : Conditionals_

_Programs often need to make decisions to execute certain actions only when specific conditions are met. This mechanism is known as **control flow**, and in Python, it is primarily managed through **conditional statement**._

_Conditional statement allow the program to evaluate expressions that result in Boolean values (```True``` or ```False```) and to choose a corresponding path of execution. This concept is fundamental to any form of logic or reasoning in programming, as it enables dynamic behavior and adaptability within code._

_The basic structure of decision-making in Python is represented by the ```if``` statement, often combined with ```elif``` (short for "else if") and ```else``` clauses. These elements together allow multiple scenarios to be tested sequentially, executing only the block that satisfies the condition._

_```age = 18```_

_```if age < 18 :```_\
_```  print("Minor")```_\
_```elif age == 18 :```_\
_```  print("Exactly eighteen")```_\
_```else :```_\
_```  print("Adult")```_

_Indentation plays a crucial role in conditionals, just as in any other Python block. Each indented group of statements represents a **suite**, which defines the actions to be taken when a condition holds true._

_Conditions can involve comparisons, logical operators, or even function calls that return Boolean values. Because of Python's dynamic typing, any object can be evaluated in a Boolean context (non-empty sequences, non-zero numbers, and most objects evaluate to ```True```, while empty structures, zero values and ```None``` evaluate to ```False```)._

#### _Nested Conditionals_

_Conditional statements can themserves contain other conditionals, forming what are known as **nested conditionals**. These are used when decisions depend on multiple levels of logic, that is when an outcome must be tested only after a previous condition has been satisfied._

_```age = 20```_\
_```citizien = True```_

_```if age >= 18 :```_\
_```  if citizen :```_\
_```    print("Eligible to vote")```_\
_```  else :```_\
_```    print("Must be a citizen to vote")```_\
_```else :```_\
_```  print("Too young to vote")```_

_Nested conditionals make complex decision trees possible, though excessive nesting can reduce readability. When logic becomes too deep, it is often better to refactor the code using logical operators (```adn```, ```or```, ```not```) or functions._

#### _Shorthand and Ternary Expressions_

_Python provides a concise syntax for writing simple conditional statements in a single line. This is known as a **ternary conditional expression**, or simply a **conditional expression**._

_```x = 18```_\
_```result = "Even" if x % 2 == 0 else "Odd"```_\
_```print(result)```_

_This compact form enhances readability when the logic is simple and both possible outcomes are short._

_A similar shorthand can be used for single ```if``` statements without an ```else```, especially when performing brief operations :_

_```x = 5```_\
_```if x > 0 : print("Positive")```_

_Although this syntax is valid, it should be used sparingly. Readability remains a core principle in Python's philosophy, and multi-line statements are usually clearer for more complex logic._

## _Control Flow : Loops_

_While conditionals allow decisions to be made once, **loops** enable a program to repeat a sequence of instructions multiple times. This repetition can continue for a specific number of iterations or until a particular condition is no longer true._
_In Python, loops are central to automation, iteration, and data processing. They eliminate redundancy by allowing tasks to be executed repeatedly with minimal code._

#### _While Loop_

_The ```while``` loop is used when the number of iterations is **not know in advance**. Execution cntinues as long as a specified condition remains true, making this structure suitable for situations where repetition depends on events or variable states that may change unpredictably during runtime._
_In essence, the ```while``` loop is ```event-driven```, reacting to conditions rather than following a fixed count._

_```count = 0```_

_```while count < 5 :```_
_```  print("count is: ", count)```_
_```  count += 1```_

_<sub>The variable ```count``` is incremented during each iteration. When it reaches 5, the condition ```count < 5``` becomes false, and the loop stops.<sub>_

_The ```while``` loop is ideal when the number of iterations is not predetermined but depends on a logical condition, such as waiting for user input or processing until a specific event occurs._

_If a ```while``` condition never becomes false, the loop continues indefinitely, this is known as an **infinite loop**. To prevent this, make sure the condition will eventually change or include a mechanism like the ```break``` statement to exit manually._

#### _For Loop_

_The ```for``` loop is typically used when the number of iterations is **known or predetermined**. It iterates over a sequence (such as list, string or range of numbers) executing the block of code once for each element._
_For this reason, the ```for``` loop is often described as **index-driven**, as its execution is guided by the progression through a defined iterable rather than by an open-ended condition._

_```fruits = ["apple", "banana", "cherry"]```_

_```for fruit in fruits :```_
_```  print(fruit)```_

_<sub>The loop variable ```fruit``` takes on each element of the list sequentially. Once all elements have been processed, the loop terminates automatically.<sub>_

_The ```for``` loop can also be used with the ```range()``` function to repeat an action a specific number of times._

_```for i in range(5) :```_
_```  print("Iteration: ", i)```_

_The ```range()``` function generates a sequence of integers starting from 0 (by default) and stopping before the specified number. It can also take optional ```start``` and ```step``` arguments._

_```for i in range(1, 10, 2):```_
_```  print(i)```_

_<sub>This example prints all odd numbers between 1 and 9 (the third parameter determines the increment, or decrement, if negative).<sub>_

_The flexibility of the ```for``` loop makes it a powerful tool for iterating over any kind of sequence or collection._

#### _Loop Control Statements_

_Loops are powerful, but sometimes it's necessary to alter their normal flow. Python provides a set of **loop control statements** that allow you to modify how and when a loop executes._

_These statements are particularly useful for handling exceptions, skipping certain iterations, or stopping the loop when a condition is met._

* _break : The ```break``` statement is used to **terminate a loop prematurely**. When Python encounters a ```break```, the loop immediately stops executing, and the control flow continues with the first statement that follows the loop._

  _```for i in range(10):```_\
  _```  if i == 5:```_\
  _```    break```_\
  _```  print(i)```_

  _<sub>The loop stops when ```i``` equals 5, even though the range goes up to 9.<sub>_

* _continue : The ```continue``` statement causes the loop to **skip the current iteration** and move directly to the next one. This is useful when certain conditions should cause the loop to ignore part of its code without breaking completely._

  _```for i in range(6):```_\
  _```  if i == 3:```_\
  _```    continue```_\
  _```  print(i)```_

  _<sub>When ```i``` equals 3, the ```continue``` statement skips that iteration, so 3 is not printed.<sub>_

* _pass : The ```pass``` statement does nothing when executed, it's simply a placeholder. It is often used when a statement is syntactically required but no action needs to be taken yet (for example, when defining an empty loop or function that will be implemented later)._

  _```for i in range(3): ```_\
  _```  pass```_

  _<sub>This loop doews nothing but remains syntactically valid.<sub>_

* _else : In Python, loops can also include an optional **else** block that executes **only if the loop completes normally**, without encountering a ```break``` statement. This is a unique feature of Python and can make the code more expressive._

  _```for i in range(5):```_\
  _```  print(i)```_\
  _```else:```_\
  _```  print("Loop finished without break.")```_

  _<sub>But if a ```break``` is triggered, the ```else``` block will be skipped.<sub>_









