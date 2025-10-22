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

