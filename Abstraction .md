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
```p
from abc import ABC, abstractmethod
import math

# Abstract Class
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

# Rectangle Class
class Rectangle(Shape):
    def __init__(self, length=10, breadth=5):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

# Circle Class
class Circle(Shape):
    def __init__(self, radius=7):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius * self.radius

# Creating Objects
rect = Rectangle()
circ = Circle()

# Displaying Areas
print("Area of Rectangle =", rect.calculate_area())
print("Area of Circle =", round(circ.calculate_area(), 2))
```
## Output
<img width="1841" height="671" alt="image" src="https://github.com/user-attachments/assets/45870452-bf9e-4bf4-9d3a-57131acd61be" />

## Result
Thus, an abstract class Shape with an abstract method calculate_area() was created, and the method was successfully implemented in the subclasses Rectangle and Circle. The areas of the rectangle and circle were calculated and displayed successfully.
