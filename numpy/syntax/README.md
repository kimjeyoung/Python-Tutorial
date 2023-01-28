NumPy is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.

Here is an example of basic syntax for creating and manipulating arrays using NumPy:

```python
import numpy as np

# Creating an array
a = np.array([1, 2, 3]) # creates an 1-dimensional array
b = np.array([[1, 2], [3, 4]]) # creates a 2-dimensional array

# Accessing elements
print(a[0]) # prints 1
print(b[0][1]) # prints 2

# Array shape
print(a.shape) # prints (3,)
print(b.shape) # prints (2, 2)

# Array reshaping
c = a.reshape(1,3) # reshapes a to a 2-dimensional array with shape (1, 3)
print(c) # prints [[1 2 3]]

# Array operations
d = np.array([4, 5, 6])
e = a + d # element-wise addition
print(e) # prints [5 7 9]

f = np.dot(b, d) # matrix multiplication
print(f) # prints [17 39]
```

This is just a simple example, NumPy is a powerful library with many other functions and features, including support for linear algebra, Fourier transform, and random number generation.

You can use it to perform mathematical operation on array, and work with matrices, it's a powerful library that can handle high-performance mathematical operations, also can handle missing values in data and it has built-in functions to handle these missing values.
