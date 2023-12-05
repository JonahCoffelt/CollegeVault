A list is a way to store multiple items in a single variable. 
___
# Creating a List
To create a list, use square brackets, with the contents of the list inside:

```python 
my_list = ['jonah', 'megan', 'ian']
my_list = [1, 2, 3, 4]
```

Items can be reassigned by simply setting an index to the new value:

```python
my_list = [1, 2, 3, 4]
my_list[1] = 5
print(my_list)

>>> [1, 5, 3, 4]
```

# Indexing
Each item in a list can be accessed through the index, starting at 0 and going up to one less than the length of the list. They can also be accessed through their negative index, which starts at -1, which is the last element, and goes to -n. 

| Index | 0   | 1   | 2   | 3   |
| ----- | --- | --- | --- | --- |
| Negative Index  | -4   | -3  | -2  | -1 |
| Item  | 3   | 42  | 23  | 25  |

For example, 42 can be accessed in the list by doing list[1] or list[-3]
## Slicing
A slice of a list is a sublist composed of some elements of a larger list. We might want to do this if we only want to access a section of a list. This is done by doing list[a:b], where is is the inclusive stating point, and b is the exclusive ending point. 

```python
my_list = [1, 2, 3, 4]
print(my_list[1:3])

>>> [2, 3]
```

If no a is provided, the slice will start at the beginning, and if no b is provided, the slice will go to the end of the list:

```python
my_list = [1, 2, 3, 4]
print(my_list[:2])
print(my_list[2:])
print(my_list[:])

>>> [1, 2]
>>> [3, 4]
>>> [1, 2, 3, 4]
```

Slicing will not give an out-of-range error, so there is no worry of putting in a value that is too small or too large. 
# List Functions
## Length
To find the length of an array, simply use the len(list) command:

```python
my_list = [1, 2, 3, 4]
print(len(my_list))

>>> 4
```

## Min/Max
The min and max functions return the least and greatest values in a list respectively:
```python
my_list = [1, 2, 3, 4]
print(min(my_list))
print(max(my_list))

>> 1
>> 4
```

## Sum
The sum function returns the sum of all the elements in a list:
```python
my_list = [1, 2, 3, 4]
print(sum(my_list))

>> 10
```
# List Operations
## Append
The append() function can add a new element to the end of a list. This is done with list.append(value):

```python
my_list = [1, 2, 3, 4]
my_list.append(5)
print(my_list)
print(len(my_list))

>>> [1, 2, 3, 4, 5]
>>> 5
```

## Concatenation
We can add list together, combine the elements into a single list:

```python
list1 = [1, 2]
list2 = [3, 4]
my_list = list1 + list2
print(my_list)

>>> [1, 2, 3, 4]
```

This can also provide an alternative to the append() function by using +=:

```python
my_list = [1, 2, 3, 4]
my_list += [5]
print(my_list)
print(len(my_list))

>>> [1, 2, 3, 4, 5]
>>> 5
```
# Looping
There are many ways to loop through a list. One way is to for a for i in range loop, with the range set to the length of the list. If the length of the list is not known before runtime, it can be found with the len() function:

```python
my_list = [1, 2, 3, 4]
for index in range(len(list)):
	print(list[index], end=' ')

>>> 1 2 3 4
```

Another way to loop through would be be accessing each element in a list, ranther then doing a range of indexes:

```python
my_list = [1, 2, 3, 4]
for element in my_list:
	print(element, end=' ')

>>> 1 2 3 4
```

## Changing a List in a Loop
For each iteration of a loop using the in list method, the element variable receives the value of the list element, but not the memory location, thus changing this variable will not change the list. 

```python
my_list = [1, 2, 3, 4]
for i in my_list:
	i = 100
print(my_list)

>>> [1, 2, 3, 4]
```

To change a list, you must actually access the item from the list:

```python
my_list = [1, 2, 3, 4]
for i in range(len(my_list)):
	my_list[i] = 100
print(my_list)

>>> [100, 100, 100, 100]
```

## Enumerate
The enumerate function provides both the index and the value of each element of a list. 

```python
my_list = [5, 4, 3, 2]
for index, value in enumerate(my_list):
	print(index, value)

>>> 0 5
>>> 1 4
>>> 2 3
>>> 3 2
```

