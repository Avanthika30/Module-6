# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class rectangle:
    def __init__(self,l,b):
        self.l=l
        self.b=b
    def get_length(self):
        return self.l
    def get_breadth(self):
        return self.b
ob=rectangle(5,3)
print(ob.get_length())
print(ob.get_breadth())
```
## Output
<img width="756" height="183" alt="image" src="https://github.com/user-attachments/assets/57009006-1673-4bdb-ab85-a80271cd8d72" />

## Result
Thus, the program has been successfully executed

