Using Modules and Packages allows programmers to utilize code that someone else has already written. Oftentimes, there is no need to reinvent the wheel, and writing some functions from scratch may be to complicated or take too long. 

# Modules
In python, a module is a single file of python code that can be used for some function. A package is simply a collection of multiple similar modules. Modules can be imported into code, giving access to all that is in it. The primary things that a module has are functions, variables, and classes.
## Importing Modules
We can import an entire module by simply using the import function. This will give us access to all the functions in the module, which are accessed in code through the module:

```python
# Importing the module  to our code
import <module name>

# Using a function in the module
<module name>.<function name>(<arguments>)
```

This is something that we have done with the math module to access trigonometric functions:

```python
import math

print(math.cos(0))

>>> 1
```

We often do not want to use the entire module though, so we can just import what we want using the from module import:

```python
from math import cos

print(math.cos(0))

>>> 1
```

If we did want to import all of the functions directly to our code, rather than through the module, it could be done with the * import:

```python
from math import *

print(math.cos(0))
print(math.sin(0))

>>> 1
>>> 0
```

### Renaming
Oftentimes, we do not want to type the entire name of a module, so we can replace it with our our name by adding "as" and the name to the end of the import:

```python
from math import cos as c

print(math.c(0))

>>> 1

```

We could do this for single functions, or the whole module:

```python
import math as m

print(m.cos(0))

>>> 1
```