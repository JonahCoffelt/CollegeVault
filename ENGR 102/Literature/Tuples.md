Tuples are similar to lists, but they are immutable. To assign a tuple, use parentheses or comma separated values:

```python
my_tuple = (1, 2, 3)
new_tuple = 1, 2, 3
```

The indexing and slicing operations are the same as for [[Lists]] 

# Tuple Operations
## Value Assignment
Values can be assigned from tuple:

```python
my_tuple = (1, 2, 3)
x, y, z = my_tuple
print(y)

>>> 2
```

If a function returns a tuple, then assignment can be done the same way:

```python
a, b = some_function()
```

