# Problem 1
> List 5 good coding practices that have been mentioned in this course.

```txt
Abstraction, bottom-up, top-down, commenting, doc-strings
```

# Problem 2
>In the following dictionary, identify the keys and values. Write the command to add the key 'Orange' with value 1 to the dictionary. Write code to loop through the dictionary and check for  a particular key or value.  

```python
mydict = {'Apple' : 3, 'Pear' : 5, 'Banana' : 2}

# Keys: 'Apple', 'Pear', 'Banana'
# Values: 3, 5, 2

mydict['Orange'] = 1

for key in mydict:
```

# Problem 3
> Explain how dictionaries are different from lists, and how lists are different from tuples.

```txt
An index is used to access a value from a list, while a key is used to access an element from a dictionary. Lists are mutable, while tuples are immutable.
```

# Problem 4
> Identify and explain 3 ways strings are similar to lists.

```txt
1) Indexing: The items of a list and a string can both be accessed through indexing
2) Slicing: Sections of both strings and lists can be retrived through index-based slicing
3) ???
```

# Problem 5
>List all of the data types we have seen in this course and provide an example of each. Identify which ones are mutable and which are immutable.

```txt
Assume all are immutable unless otherwise stated
1) int: An integrer number (4)
2) float: A number with a floating point/decimal (2.3)
3) string: A sqeunce of characters ("word")
4) list (Mutable): A sqeuence of like items ([1, 2, 3])
5) dict (Mutable): A sqeucnce of key value pairs ({'key' : 1})
6) tuple: Like an immutable list ((1, 2, 3))
```

# Problem 8
> Does it matter if we use the same variable names inside a user defined function and the main program? Why (not)?

```txt
It does not matter, because the main memory space is sperate from the function memory space.
```

# Problem 9
> Does it matter where in our code we write function definitions?

```txt
Yes, they must be at the top.
```

# Problem 15
> What are the differences between myfile.read(), myfile.readline(), myfile.readlines(), and list(myfile)?

```txt
1) read() - Gives the entire file as a string
2) readline() - Only gives one line as a string
3) readlines() - Gives a list of all lines
4) list(myfile) - Gives a list of all lines
```

# Problem 17
> Write the command to print the value of pi to 4 decimal places to the screen. Don’t forget to import pi from the math module!

```python
from math import pi

print(f'{pi:.4f}')
```

# Auto Graded
22) Error
23) ("Howdy", [2, 0, 2, 7])
24) 3
25) This function prints a message.
26) 6
27) 2 Too big!
28) Error
29) Hi Ann
30) :
```txt
Length: 5
Max: 5
Min: 5
Crazy: 3
```
31) Howdy Texas A&M Engineering students!
32) 1 2 3 5 7 9 
33) x is the float .5
