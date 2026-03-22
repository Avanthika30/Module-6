# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```
class A:
    def __init__(self, a):
        self.a = a
    def __lt__(self, other):
        return self.a<other.a
ob1 = A(20)
ob2 = A(3)
if (ob1<ob2):
    print("ob1 is less than ob2")
else:
    print("ob2 is less than ob1")
```
## Output
<img width="1145" height="166" alt="image" src="https://github.com/user-attachments/assets/3b8c3df1-d4ee-4422-8ac1-eb772dc67b53" />

## Result
Thus, the program has been successfully executed
