# Exp.No:29  
## Encapsulation

---

### AIM  
To write a Python program to create a class `Student` with the private members `name` and `age`, and add getter and setter methods to initialize and modify the `age` variable.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the `Student` class.**
   - Inside the `Student` class, define the `__init__` method to initialize `name` and the private member `__age`.
3. **Define a getter method** `get_age` to return the value of the private member `__age`.
4. **Define a setter method** `set_age` to set a new value to the private member `__age`.
5. **Create an object `stud`** of the `Student` class with the name 'Jessa' and age 14.
6. **Print the name and the age** of `stud` using the getter method.
7. **Use the setter method** `set_age` to change the age of `stud` to 16.
8. **Print the name and the updated age** of `stud` using the getter method.
9. **End the program.**

---

### PROGRAM

```python
class Student:
    def __init__(self, name, age):
        self.__name = name
        self.__age = None
        self.set_age(age)  # Use setter to initialize

    # Getter for age
    def get_age(self):
        return self.__age

    # Setter for age
    def set_age(self, age):
        if age > 0:
            self.__age = age
        else:
            print("Invalid age")

    # Method to display student details
    def show(self):
        print(f"Name: {self.__name} {self.__age}")

# Example usage
s = Student("Jessa", 14)
s.show()

s.set_age(16)
s.show()


```

### OUTPUT
<img width="559" height="171" alt="image" src="https://github.com/user-attachments/assets/084bb9f4-84dd-4496-b22d-a1f86ed1f36d" />



### RESULT
Thus the python program to create a class `Student` with the private members `name` and `age`, and add getter and setter methods to initialize and modify the `age` variable has been implemented and executed successfully.
