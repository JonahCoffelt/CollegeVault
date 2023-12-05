(To be filled in at a later date)

# String Processing
## Split
We may want to break a string into parts to be easily used. To do this, we can use the split() function. This creates a list of strings based on a specified separator. Here is the basic format:

```python
<list> = <str>.split('<str to split on>')
```

Here is an example:

```python
my_str = '1,2,3,4'
elements = my_str.split(',')
print(elements)

>>> ['1', '2', '3', '4']
```

## Join
The join function is like the opposite of the split function, it can join a list of strings into a single string, with a separator in between each element. Here is the basic format:

```python
'<str separator>'.join(<list>)
```

For example:

```python
print('.'.join(['1', '2', '3', '4']))

>>> 1.2.3.4
```

## Strip
The strip() function can be used to remove leading and trailing white space, such as spaces and line ends:

```python
print('|' + '  1, 2, 3   \n'.strip() + '|')

>>> |1, 2, 3|
```
