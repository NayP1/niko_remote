---
id: 24kh5oujri960rnvnkjgx3p
title: arange method
desc: ''
updated: 1676963283273
created: 1676963070019
---
```np.arange()``` is a method provided by the NumPy library in Python, which creates an array of evenly spaced values within a specified interval.

The method takes in three arguments: start, stop, and step.

Examples:

```python
import numpy as np

# Create an array of values from 0 to 9
arr = np.arange(10)
print(arr)  # [0 1 2 3 4 5 6 7 8 9]

# Create an array of values from 1 to 10 with a step of 2
arr = np.arange(1, 11, 2)
print(arr)  # [1 3 5 7 9]

# Create an array of values from 10 to 1 with a step of -1
arr = np.arange(10, 0, -1)
print(arr)  # [10 9 8 7 6 5 4 3 2 1
```