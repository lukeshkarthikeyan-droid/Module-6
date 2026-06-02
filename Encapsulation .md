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
```p
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth

    def display(self):
        print("Length =", self.__length)
        print("Breadth =", self.__breadth)

# Creating an object
rect = Rectangle(10, 5)

# Accessing private variables through a method
rect.display()
```
## Output
<img width="1850" height="524" alt="image" src="https://github.com/user-attachments/assets/ee9acbf7-5d80-477e-8c31-f0c38fa1f921" />

## Result
Thus, the Python program to demonstrate Encapsulation using private member variables __length and __breadth in a Rectangle class was implemented and executed successfully.
