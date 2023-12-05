# Pyplot
## Intro
To import Pyplot, use the following import:

```python
import matplotlib.pyplot as plt
```

With this, we can do some basic plotting. For example, we can plot an array of data:
```python
plt.plot([1, 2, 3, 4])
plt.show()
```
![[Figure_1.png|500]]

In this example, since we only provided a single array, Pyplot assumed that we gave it the y values, thus the x-axis will be in indices: [0, 1, 2, 3]

We can specify both axes by providing two arrays:
```python
plt.plot([1, 2, 3, 4], [1, 4, 9, 16])
```
![[Figure_1 2.png|500]]

## Formatting
After giving the data, the style of the points can be specified. This is done through a string that has the color followed by the drawing type. The default is 'b-' which means a solid blue line. Here is an example of red circles:
```python
plt.plot([1, 2, 3, 4], [1, 4, 9, 16], 'ro')
```
![[Figure_1 3.png]]

Here are some common colors and line types:

**Colors**:
- 'k' - Black
**Lines & Markers**:
- '-' - Solid line
- '--' - Dashed line
- ':' - Dotted line
- 'o' - Circle marker
- 'v' - Downward triangle
- '^' - Upward triangle
- 's' - Square marker
- 'D' - Diamond Marker
- 'd' - Thin diamond Marker
- '\*' - Star marker
- '+' - Plus marker
- 'x' - Cross marker

The axis of the plot can be specified with the axis() function, which takes in a tuple for (xmin, xmax, ymin, ymax):
```python
plt.plot([1, 2, 3, 4], [1, 4, 9, 16], 'g*')
plt.axis((0, 10, 0, 40))
```
![[Figure_1 4.png]]
