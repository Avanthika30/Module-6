# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
class Beans:
    def type(self):
        return "Vegetable"
    def color(self):
        return "Green"
class Mango:
    def type(self):
        return "Fruit"

    def color(self):
        return "Yellow"
def describe(obj):
    print(obj.type())
    print(obj.color())
beans1 = Beans()
mango1 = Mango()
describe(beans1)
describe(mango1)
```
## Output
<img width="1136" height="230" alt="image" src="https://github.com/user-attachments/assets/74ffbd0a-6662-44f4-9a4b-1ff185dbf76b" />

## Result
Thus, the program has been successfully executed.
