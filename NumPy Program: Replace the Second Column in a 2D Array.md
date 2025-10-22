# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```py
import numpy as np
a=np.array([[1,2,3,4,5],[6,7,8,9,5],[3,4,6,8,3]])
c=np.array([10,5,15])
k=np.delete(a,1,axis=1)
h=np.insert(k,1,c,axis=1)
print(h)
```

## Output
<img width="1515" height="343" alt="image" src="https://github.com/user-attachments/assets/38a9c3c3-1403-40b5-90d3-7a41f4d978a2" />

## Result
successfully wrote **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.
