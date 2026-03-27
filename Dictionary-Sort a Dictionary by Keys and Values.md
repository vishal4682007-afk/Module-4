# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
dict = {'b':1,'e':27,'c':7,'a':3,'d':15}

# To sort dictionary by keys
sort1 = sorted(dict.items())
print("The Sorted Dictionary by keys.....")
dict1={}
for key,value in sort1:
    dict1[key] = value
print(dict1)

print()

# To sort dictionary by values
sort2 = sorted(dict.items(),key = lambda item : item[1])
print("The Sorted Dictionary by values.....")
dict2 = {}
for key,value in sort2:
    dict2[key] = value
print(dict2)

## Sample Output
<img width="1918" height="842" alt="image" src="https://github.com/user-attachments/assets/3c320c1f-4a95-40cc-baba-814273fa0f6b" />


## Result
Thus, The To write a Python program that sorts a dictionary according to its Keys in alphabetical order and to its Values in alphabetical order was executed successfully.
