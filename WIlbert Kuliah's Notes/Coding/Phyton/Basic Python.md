# Basic Python

## Introduction
---
#### Data Type
Python have several kinds of *Data Types* which includes :
- Text Type: `str`
- Numeric Types: `int`, `float`, `complex`
- Sequence Types: `list`, `tuple`, `range`
- Mapping Type: `dict`
- Set Types: `set`, `frozenset`
- Boolean Type: `bool`
- Binary Types: `bytes`, `bytearray`, `memoryview`
- None Type: `NoneType`

#### Variables
*Variables* is a way to store data in Python, you can create a variable by creating an identifier. After that you can assign a value to the identifier. For example
```python
a = 10
b = "abcd"
```

#### Operators
Operators in Python is seperated to a few types :

##### Arithmatic Operator
Arithmatic Operator is the normal mathematical operator that consist of 
- Addition : `+`
- Subtraction : `-`
- Multiplication : `*`
- Division : `/`
- Modulus : `%`
- Exponentiantion : `**`
- Floor Division : `//`

##### Comparison Operator
Comparison Operator is used to compare 2 values :
- Equal : *==
- Not Equal : **!=**
- Bigger Than : **>**
- Smaller Than : **<**
- Bigger Than or Equal to : **>=**
- Smaller Than or Equal to : **<=**

##### Logical Operator
Logical Operator is the operator to combine conditional statement that consist of
- and
- or
- not

#### Conditional
You can make a conditional statement in Python by using the if, else, elif syntax. For example
```Python
a = 10
b = 11

if (a == 10) :
	print(a)
elif (b == 1) :
	print(b)
else :
	print(a + b)
```

#### Loop
Looping is used to loop a block of code for the sake of efficiency. There are 2 types of loop in Python, that is 

##### While Loop
While Loop is used by specifying a conditional and if that condition is *True* than it will keep looping until it's *False*. For example
```python
While True:
	print("10")
```

##### For Loop
For Loop is used by specifying a limit to the loop. The limit can be a the length of character, the size of list or array, and much more. For example
```python
for a in range(10):
	print('1')
```

#### Storing a Collection of Data
There a 4 Data Types to store a collection of data in a single variable. That is 

##### Lists
Lists are used to store multiple items in a single variable. Lists are created using square brackets. For example
```python
thislist = ['apple', 'banana', 'orange']
```

##### Tuples
Tuples are used to store multiple items in a single variable. A tuple is a collection which is ordered and **unchangeable**. Tuples are written with round brackets. For example
```python
thisTuple = ("apple", "banana", "orange")
```

##### Sets
Sets are used to store multiple items in a single variable. A set is a collection which is _unordered_, _unchangeable_, and _unindexed_. For example
```python
thisset = {"apple", "banana", "cherry"}
```

##### Dictionary
Dictionaries are used to store data values in key:value pairs. A dictionary is a collection which is *ordered*, *changeable* and *do not allow duplicates*. Dictionaries are written with curly brackets, and have keys and values. For example
```python
thisdict = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}
```

#### Modules
A module is a set of function that you can use. You can create your own module and there are also built-in module in python. to use a module you must use `import` keyword. For example to import the math module like this
```python
import math
```

You can also import specific function from a module using the keyword `from` and `import` simultaneously. For example
```python
from math import sqrt
```

Here are some frequently used module in Python :
- [[Numpy]]
- [[Matplotlib.pylot]]
- [[Pandas]]