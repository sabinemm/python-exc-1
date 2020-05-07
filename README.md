# Python Notes
python3 to start
ctrl + D to exit

## Significant Whitespace

1. Prefer four spaces (standart)
2. **Never** mix tabs and spaces
3. Be consistent with consecutive lines
4. Has exceptions

Code blocks are initiated with a **:** 

    and comprised of lines

    with the

    same

    indentation

    LVL

Programming as Guido indented it.

## Python Culture
PEP 8 - how to format your code

PEP 20 - Zen of Python 
```
ìmport this
```

Beautiful is better than ugly.

Explicit is better than implicit.

Simple is better than complex.

Complex is better than complicated.

Flat is better than nested.

Sparse is better than dense.

Readability counts.

Special cases aren't special enough to break the rules.

Although practicality beats purity.

Errors should never pass silently.

Unless explicitly silenced.

In the face of ambiguity, refuse the temptation to guess.

There should be one-- and preferably only one --obvious way to do it.

Although that way may not be obvious at first unless you're Dutch.

Now is better than never.

Although never is often better than *right* now.

If the implementation is hard to explain, it's a bad idea.

If the implementation is easy to explain, it may be a good idea.

Namespaces are one honking great idea -- let's do more of those!

## Using the Standard Library
Also called Batteries Included

    import_module
```
import math
```
module_name.attribute_name

to get help simply type help, arrow keys on Mac to browse. Press Q to return to REPL

Type module first for clarity.
```math.factorial(5)```

Shorter:
```
from math import factorial as fac
```
Don't use often

## Scalar types, Operators, and Control Flow

Scalar Types

### **int** 
42 whole numbers arbitrary precision integer

int unlimited precision signed integer - can contain as many digits you need

binary - 0b10

octal - 0o10

hexadecimal - 0x10

int(3.5) >>> 3

int(-3.5) >>> 3

Always rounds towards 0

### **float** 
4.2 64 bit floating point numbers

15-16 significant digits in decimal

numbers written with a decimal are automatically floats
In Python 3, whenever we use the division operator, the result will always be a float. For example: 15/3 = 5.0
### **NoneType** 
None the null object. Placeholder value

Printing None into REPL has no effect. 

Can be bound to variable names 
```
a = None
a is None
True
```
### **bool** 
True/False Boolean logic values

### Basic use of relational operators
### Basic flow-control mechanisms

## Operator Precedence
When the computer processes a mathematical expression with these operations, it follows these steps:

1. If the expression has any bracketed parts, start with the sub-expressions inside of these first 
2. Calculate any exponents
3. Calculate multiplication and division - these 2 operations have the same precedence, since division is treated as multiplying by the reciprocal number
4. Calculate addition and subtraction - these 2 operations have the same precedence, since subtraction is treated as adding the negative number
5. If we were dealing with a sub-expression, get rid of the brackets now and proceed to calculate the outer expression, when only a single number is left, we're done
## Variables
The equals sign is known as the **assignment operator.** We use this when we wish to assign values to a variable.

Python comes with it’s standard for writing readable code called [PEP8](https://www.python.org/dev/peps/pep-0008/). This standard only acts as guidelines for how code should be written to make all code as readable to all Python developers. PEP8 recommends using lowercase variable names and any variable names that contain spaces should use underscores as spaces.

Function names should be lowercase, with words separated by underscores as necessary to improve readability.

Variable names follow the same convention as function names.

mixedCase is allowed only in contexts where that's already the prevailing style (e.g. threading.py), to retain backwards compatibility.

## Working With Numbers

But what if we wanted to do some division that just returns an int instead? In that case, we would use the floor division operator. Back in the Arithmetic Operators section, we saw a floor division operator that looked like this –//. It rounds the number down to the nearest whole number.

If we add an int to a float, the result will be a float.

Any arithmetic operation that involves an int and a float as its operands behaves the same. However, if we were to perform an arithmetic operation on two ints, then the result will be an int. Similarly, if we use two floats as our operands, then the result will be a float.

Remember that there are a few rules in python when it comes to combining integers and floats in different ways:

Floats combined with floats will always return a float
Integers combined with floats will always return a float
Integers combined with integers will always return an integer
Use of the division (/) operator always results in a float
Use of the floor division (//) operator can return either an integer or a float, depending on its operands

### Rounding
Here we’ve stored the converted and rounded value in a variable called total_usd. The first argument that we pass to the round function is the value that we need to be rounded, and the second argument is the number of decimal points that we want to round to. In this case, we want to round to two decimal places.

``` 
usd = 1.11
euro = 25
total_usd = round(euro * usd, 2)
print(total_usd)
```

### Input
```
name = input("What's your name? ")
age = input("What's your age: ")
print("Hello %s, you are %s years old" %(name, age))
print("Hello {}, you are {} years old".format(name, age))
```

When formatting with f-strings you would do the following: f"{variable}"
It is also valid to use the capital letter F
The only consideration required to use f-strings is your version of python, which needs to be version 3.6 or above.
Let's look at an example below.
```
name = input("What's your name? ")
# Here we don't need age to be a number as we are not
# going to do any calculations with it so we don't need to wrap the
# input() in the str() method
age = input("What's your age: ")

# The Modern way of formatting a string
print(f"Hello {name}, you are {age} years old")
```

## FLASK
sudo pip3 install Flask
dependecies pip3 freeze --local > requirements.txt

 sudo pip3 install -r requirements.txt to install dependencies
 And the -r switch just tells pip to install from the requirements.txt file, rather than looking at the package index.