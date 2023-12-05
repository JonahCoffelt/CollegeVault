A function is a section of code that is separated from the main file. Call functions move the interpreter to the function, then bring it back to the same place once the function code has fully executed or exited. 

> But why write functions?

Functions can help to prevent rewriting of sections of code, can conceptually separate aspects of code, and can be executed separately from the rest of the code. 

# Calling Functions
Functions can be called with like this: name(arguments). For example, the print() function has a name, "print", as well as a string argument for what to print. 
## Arguments
Arguments are useful because functions do not have access to the data in the main code. All data needed should be passed to the function via arguments. Multiple arguments can be separated by commas:

```python
print(1, 2)

>>> 1 2
```

## Return
Data can be returned from the function back to the main code through a return value. For example, the sqrt() function takes in a number as an argument, then returns the value of its square root to the main code:

```python
from math import sqrt

x = 4
sqrt_of_x = sqrt(x)
print(sqrt_of_x)

>>> 2
```

Multiple values can be returned by using [[Tuples]], lists, or strings, though most commonly a tuple is used. 