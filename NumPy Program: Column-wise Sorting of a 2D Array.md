# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```py
import numpy as np
a=np.array([[1,5,8,6],[5,8,4,3]])
c=np.sort(a,axis=0)
print("array:",a)
print("sorted array:",c)
```
## Output
<img width="1257" height="230" alt="image" src="https://github.com/user-attachments/assets/f0d6b50f-4681-47ce-8c6b-e52085994be4" />

## Result
successfully wrote **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.
