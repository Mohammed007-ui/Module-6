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

```
class Student:
    def __init__(self, name, age):
        self.name = name
        self.__age = age  # Private member __age

    # Getter method to retrieve the age
    def get_age(self):
        return self.__age

    # Setter method to modify the age
    def set_age(self, age):
        self.__age = age

# Create a Student object with name 'Jessa' and age 14
stud = Student("Jessa", 14)

# Print the name and the age using the getter method
print(f"Name: {stud.name}, Age: {stud.get_age()}")  # Output: Name: Jessa, Age: 14

# Use the setter method to change the age to 16
stud.set_age(16)

# Print the name and the updated age using the getter method
print(f"Name: {stud.name}, Age: {stud.get_age()}")  # Output: Name: Jessa, Age: 16

```

### OUTPUT
![image](https://github.com/user-attachments/assets/9171056a-2cf0-461c-a53d-dc760d3c73eb)


### RESULT
The program successfully demonstrates the use of encapsulation by creating a Student class with private members (name, age). Getter and setter methods are used to access and modify the private age attribute.

