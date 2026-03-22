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

