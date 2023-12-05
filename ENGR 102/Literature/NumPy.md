# The Basics
NumPy's main object is the homogeneous multidimensional array. This is a table of numbers. Below is an example of an array with two axes, with the first axis of length 2 and the second axis of length 3:

```python
[[1., 0., 0.],
 [0., 1., 2.]]
```

The array object has the following important attributes:
- array.ndim - The number of axes
- array.shape - The dimensions of an array as a tuple
- array.size - The total number of elements
- array.dtype - The data type of the element values

## Array Creation
There are may ways to create an array. One of the most simple is to convert a python array to a NumPy array:

```python
>>> import numpy as np
>>> a = np.array([1, 2, 3])
>>> print(a)
array([1, 2, 3])
>>> print(a.dtype)
dtype('int64')
```

The NumPy array will transform a sequence of lists into a 2D array:

```python
>>> b = np.array([(1.5, 2, 3), (4, 5, 6)])
>>> print(b)
array([[1.5, 2. , 3. ],
       [4. , 5. , 6. ]])
```

The np.zeros(), np.ones(), and np.empty() functions can all create similar arrays by taking in a shape as an argument:

```python
>>> np.zeros((3, 4))
array([[0., 0., 0., 0.],
       [0., 0., 0., 0.],
       [0., 0., 0., 0.]])
>>> np.ones((2, 3, 4), dtype=np.int16)
array([[[1, 1, 1, 1],
        [1, 1, 1, 1],
        [1, 1, 1, 1]],
```

The arange function creates a list in a similar way to the python range function, taking in a starting point, ending point, and step size:

```python
>>> np.arange(10, 30, 5)
array([10, 15, 20, 25])
```

The linspace function will create n amount of points between the start and end, rather than taking in a step size:

```python
>>> np.linspace(0, 2, 9)
array([0.  , 0.25, 0.5 , 0.75, 1.  , 1.25, 1.5 , 1.75, 2.  ])
```

## Basic Operations
