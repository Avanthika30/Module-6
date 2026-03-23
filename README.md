# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC,abstractmethod
class type_shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Rectangle(type_shape):
    def __init__(self,length,breadth):
        self.length=length
        self.breadth=breadth
    def area(self):
        print("Area of a rectangle:",self.length * self.breadth)
class Circle(type_shape):
    def __init__(self,radius):
        self.radius=radius
    def area(self):
        print("Area of a circle:",round(3.14*self.radius*self.radius,2))
class Square(type_shape):
    def __init__(self,side):
        self.side=side
    def area(self):
        print("Area of a square:",self.side*self.side)
class Triangle(type_shape):
    def __init__(self,base,height):
        self.base=base
        self.height=height
    def area(self):
        print("Area of a triangle:",0.5*self.base*self.height)
r=Rectangle(6,4)
c=Circle(7)
s=Square(4)
t=Triangle(5,4)
r.area()
c.area()
s.area()
t.area()
```
## Output
<img width="1097" height="217" alt="image" src="https://github.com/user-attachments/assets/2f3a7d5a-748b-4dcf-b9fe-fb75b5493a41" />

## Result
Thus, the program has been successfully executed.

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

# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```
class Fish:
def type(self):
print("fish")
class Shark(Fish):
def type(self):
print("shark")
obj_goldfish=Fish()
obj_hammerhead=Shark()
for animal in(obj_goldfish,obj_hammerhead):
animal.type()
```
## OUTPUT
<img width="839" height="289" alt="image" src="https://github.com/user-attachments/assets/41f351e6-4fa8-4184-a322-4bdcc104fa86" />

## RESULT
Thus, the program has been successfully executed.

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
