# Python Notes
python3 to start
ctrl + D to exit

## Significant Whitespace

1. Prefer four spaces (standart)
2. **Never** mix tabs and spaces
3. Be consistent with consecutive lines
4. Has exceptions

Code blocks are initiated with a : 
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
