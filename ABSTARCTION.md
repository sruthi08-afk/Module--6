# Exp.No:28  
## Abstraction

---

### AIM  
To write a Python program to define the abstract base class named `Polygon` and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the `sides()` method.

---

### ALGORITHM

1. **Start the Program.**
2. **Import the ABC class** from the `abc` module to implement abstraction.
3. **Define the abstract base class Polygon**:
   - Inherit from `ABC` (Abstract Base Class).
   - Define an abstract method `sides()` with no implementation.
4. **Define the Triangle class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Triangle has 3 sides"`.
5. **Define the Pentagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Pentagon has 5 sides"`.
6. **Define the Hexagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Hexagon has 6 sides"`.
7. **Define the Square class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"I have 4 sides"`.
8. **Create an object `t` of the Triangle class** and call the `sides()` method to print the number of sides.
9. **Create an object `s` of the Square class** and call the `sides()` method to print the number of sides.
10. **Create an object `p` of the Pentagon class** and call the `sides()` method to print the number of sides.
11. **Create an object `k` of the Hexagon class** and call the `sides()` method to print the number of sides.
12. **End the Program.**

---

### PROGRAM

```python
from abc import ABC, abstractmethod

# Abstract base class
class Polygon(ABC):

    @abstractmethod
    def sides(self):
        pass

# Triangle class
class Triangle(Polygon):
    def sides(self):
        print("Triangle has 3 sides")

# Quadrilateral class
class Quadrilateral(Polygon):
    def sides(self):
        print("I have 4 sides")

# Pentagon class
class Pentagon(Polygon):
    def sides(self):
        print("Pentagon has 5 sides")

# Hexagon class
class Hexagon(Polygon):
    def sides(self):
        print("Hexagon has 6 sides")

# Create objects and invoke the method
t = Triangle()
t.sides()

q = Quadrilateral()
q.sides()

p = Pentagon()
p.sides()

h = Hexagon()
h.sides()



```
### OUTPUT
<img width="501" height="273" alt="image" src="https://github.com/user-attachments/assets/61506ac5-2238-4b84-b5a9-97688ce61601" />



### RESULT
Thus the python program to define the abstract base class named `Polygon` and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the `sides()` method has been implemented and executed successfully.
