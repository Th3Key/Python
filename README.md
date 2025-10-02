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

_The syntax of Python distinguishes it from many other languages. **Indentation** is used to define the structure of code, replacing the braces or keywords that are common elsewhere. The result is source code that is clean, uniform, and immediately comprehensible._\
_Another defining aspect of Python is its **dynamic typing system**. Variables do not need to be declared with explicit types; the type is inferred automatically at runtime. At the same time, Python maintains strong rules for type behavior, ensuring that values behave predictably even in the absence of explicit declarations._\
_It is also **case-sensitive**, meaning that identifiers with different letter cases are treated as distinct names (**keywords** are fixed in lowercase)._

_The language does not confine developers to a single paradigm. **Procedural programming**, **Object-Oriented design**, and **Functional constructs** can coexist within the same project. This versatility allows Python to adapt to a wide variety of domains, from small scripts that automate routine tasks to large systems that require complex architectures._

_A significant advantage of Python lies in its comprehensive **standard library**. Modules for mathematics, file manipulation, networking, and system interaction are included with every installation. Beyond this foundation, the **Python Package index** provides access to thousands of external libraries, extending the language into specialized fields._

_Python is also **platform-independent**, working consistently across Windows, macOS, and Linux environments. This portability simplifies deployment and collaboration, ensuring that code developed in one context can easily be executed in another. The **open-source** nature of the language has cultivated an exceptionally large and active community, which contributes documentation, tutorials, and improvements to the ecosystem._

## _Variables and Data Types_

_A variable in Python is a symbolic name that stores data in memory. Variables act as containers for values, allowing programs to work with data in a flexible way. In Python, variables are created the moment a value is assigned to them (there is no need to declare their type explicitly)._

_```name = "Chris"```_\
_```age = 25```_

_<sub>**name** stores a string<sub>_\
_<sub>**age** stores an integer<sub>_

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
* _**Subtraction**: ```-```_
* _**Multiplication**: ```*```_
* _**Division**: ```/``` (always returns a float, even when dividing integers)_
* _**Floor Division**: ```//``` (returns the integer quotient, discarding the remainder)_
* _**Modulo**: ```%``` (returns the remainder of a division)_
* _**Exponentiation**: ```**``` (raises a number to the power of another)_

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











