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
