## Sridhar (25017646)

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

# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```py
import numpy as np
x=np.array([21,18,45,63,78,86,75])
y=np.array([21,12,15,35,45,56,46])
c=np.where(x>y)
k=np.where(x==y)
print(c)
print(k)
```

## Output
<img width="1536" height="387" alt="image" src="https://github.com/user-attachments/assets/58b30d30-16e7-43be-a091-e9572196d0fc" />

## Result
successfully wrote Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.
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

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```py
import pandas as pd
import numpy as np
data={
    "name":["sridhar",'mg','isravel','nandha','balamurugan'],
'score':[12.5,9.5,9.65,9.95,10.54],
'attempt':[1,2,3,2,1],
'qualify':['yes','no','yes','no','yes']}
labels=['a','b','c','d','e']
c=pd.DataFrame(data ,index=labels)
print(c)

```

## Output
<img width="1505" height="357" alt="image" src="https://github.com/user-attachments/assets/bc2ed102-0fa2-4d80-a494-a56c3a7af486" />


## Result
successfully wrote **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```py
import pandas as pd
data={
    "name":["sridhar",'mg','isravel','nandha','balamurugan'],
'score':[12.5,9.5,9.65,9.95,10.54],
'attempt':[1,2,3,2,1],
'qualify':['yes','no','yes','no','yes']}
labels=['a','b','c','d','e']

data1={
    "name":["muruga",'deva','sekar','siva','deva'],
'score':[12.8,10.2,11.2,9.45,10.54],
'attempt':[1,3,2,1,2],
'qualify':['yes','yes','no','no','yes']}
c=pd.DataFrame(data)
l=pd.DataFrame(data1)
m=pd.concat([c,l],axis=0)
print(m)
```

## Output
<img width="1435" height="516" alt="image" src="https://github.com/user-attachments/assets/4d3fcb7a-bda9-4189-8494-db9fee4d1041" />

## Result
successfully wrote Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.
