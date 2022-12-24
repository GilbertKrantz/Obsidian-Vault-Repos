# Numpy
## Import Numpy
```python
import Numpy as np
```
---

## Code

### Types of Array
#### Vector
**Create a Vector**
Designate the name of the vector as the Variable name, then use ***np.array*** to make it an array and then only use 1 brackets.
```python
Vector = np.array([1, 2, 3])
```
---

#### Matrix
**Create a Matrix**
Designate the name of the Matrix, then use ***np.array*** to make it an array and then put a *main bracket* and then put a bracket inside it for the *first array* and so on.
```python
Matrix = np.array([
				   [1, 2, 3],
				   [4, 5, 6],
				   [7, 8, 9]
])
```

**Matrix Inspection**
Functions to Inspect the **Properties of an Matrix**. Inspection includes what *dimension* is the array in, the *shape* of the matrix, the *size* of the matrix, the *length* of the matrix, and much more.
```Python
A.ndim

A.shape

A.size

len(A)
```

**Matrix Slicing**
Syntax to *Slice a Matrix* and get the value of the matrix from it. You can call a Value or even multiple Value from it
```Python
A = np.array([1,2,3,4,5,6])
B = np.array([[1,2,3,4], [5,6,7,8], [9,10,11,12]])

print(A[1]) #Call a value from a vector based on the index, start from 0
print(A[1:3]) #Call multiple value from a vector basec on the start index and ending on the end index, counting from 0

print(B[1,2]) #Call a value from a matrix based on the dimension index, start from 0 dimension and 0 index
print(B[1:3, 1:3]) #Call multiple value from a matrix base on the start dimension index and ending on the end of the dimension index, counting from 0
```

##### Matrix Operation
**Mathematical Operation**
Mathematical Operation for Matrix like +, - . *
```Python
A = np.array([[1,2,3], [4,5,6]])
B = np.array([[2,3,4], [5,6,7]])

A + B
A - B
A * B
```

**Concatenate** 
A Function to *Combine* 2 Matrixes into 1 Matrix by their axis. to add on the Y dimension and 1 to add on the X dimension.
```Python
C = np.concatenate((A,B), axis=0)
D = np.concatenate((A,B), axis=1)
```

**Transpose**
A Function to *Transpose* a Matrix. it made the Value on the X axis into Y and vice versa.
```Python
array.transpose()
```

**Reshape**
A function to *Reshape* a Matrix by according to X and Y. *(Matrix value must be enough to fill all spots and not more)**
```python
A.reshape(X, Y)
```

**Ravel**
A Function to *Ravel* a Matrix into a single line Vector.
```Python
array.ravel()
```
---

#### Tensor
**Create a Tensor**
Designate the name of the Tensor, then use ***np.array*** to make it an array and then put a *main bracket*  for the *1st Dimension* and then put a bracket inside it for the *2nd Dimension*  and then put a bracket inside it for the *first array* and so on.
```Python
Tensor = np.array([
				   [[1, 2, 3],
				   [4, 5, 6],
				   [7, 8, 9]],
				   [[10, 11],
				   [12, 13],
				   [14, 15]]
])
```
---
#### Linear Algebra

##### Dot Product
-    both _a_ and _b_ are 1-D arrays, it is inner product of vectors (without complex conjugation).
    
-   If both _a_ and _b_ are 2-D arrays, it is matrix multiplication, but using [`matmul`](https://numpy.org/doc/stable/reference/generated/numpy.matmul.html#numpy.matmul "numpy.matmul") or `a @ b` is preferred.
    
-   If either _a_ or _b_ is 0-D (scalar), it is equivalent to [`multiply`](https://numpy.org/doc/stable/reference/generated/numpy.multiply.html#numpy.multiply "numpy.multiply") and using `numpy.multiply(a, b)` or `a * b` is preferred.
    
-   If _a_ is an N-D array and _b_ is a 1-D array, it is a sum product over the last axis of _a_ and _b_.
    
-   If _a_ is an N-D array and _b_ is an M-D array (where `M>=2`), it is a sum product over the last axis of _a_ and the second-to-last axis of _b_
```Python
dot(a, b)[i,j,k,m] = sum(a[i,j,:] * b[k,:,m])
```

##### Linalg
**Determinant**
Computing the Determinant of an array
```Python
a = np.array([[1, 2], [3, 4]])
np.linalg.det(a)
```

**Inverse**
Compute the (multiplicative) inverse of a matrix.
```Python
A_inv = np.linalg.inv(A)
```
---

#### Statistics

**Mean**
Compute the arithmetic mean along the specified axis.
```Python
arrayMean = np.mean(my_array)
```

**Median**
Compute the median along the specified axis.
```Python
arrayMedian = np.median(my_array)
```

**Variance**
Compute the variance along the specified axis.
```Python
arrayVariance = np.var(my_array)
```

**Strandart Deviation**
Compute the standard deviation along the specified axis.
```Python
arrayStd = np.std(my_array)
```

**Percentile**
Compute the q-th percentile of the data along the specified axis.
```Python
arrayPercentile = np.percentile(my_array, [25, 50, 75])
```

**Quantile**
Compute the q-th quantile of the data along the specified axis.
```Python
arrayQuantile = np.quantile(my_array, [0.25, 0.5, 0.75])
```