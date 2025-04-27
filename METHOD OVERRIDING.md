# Exp.No:26  
## Method Overriding

---

### AIM  
To write a Python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()`. Create an object for each class and call the methods of the class which will print the name of the bird that is flying.

---

### ALGORITHM

1. **Begin the program.**
2. **Define the Bird class**:
   - Create a method `intro()` to print "There are many types of birds."
   - Create a method `flight()` to print "Most of the birds can fly but some cannot."
3. **Define the Sparrow class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Sparrows can fly."
4. **Define the Ostrich class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Ostriches cannot fly."
5. **Create an object `obj_bird`** of the `Bird` class.
6. **Create an object `obj_spr`** of the `Sparrow` class.
7. **Create an object `obj_ost`** of the `Ostrich` class.
8. **Print the general message** "There are many types of birds."
9. **Call the `flight()` method** on each object (`obj_bird`, `obj_spr`, `obj_ost`) to display the respective messages.
10. **Terminate the program.**

---

### PROGRAM

```
# Parent class
class Bird:
    def intro(self):
        print("There are many types of birds.")
        
    def flight(self):
        print("Most of the birds can fly but some cannot.")

# Child class Sparrow
class Sparrow(Bird):
    def flight(self):
        super().intro()  # Calling the intro() method of the parent class
        print("Sparrows can fly.")

# Child class Ostrich
class Ostrich(Bird):
    def flight(self):
        super().intro()  # Calling the intro() method of the parent class
        print("Ostriches cannot fly.")

# Creating objects of each class
obj_bird = Bird()
obj_spr = Sparrow()
obj_ost = Ostrich()

# Calling the methods
obj_bird.intro()
obj_bird.flight()

obj_spr.flight()

obj_ost.flight()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/e27e35b0-6710-402e-84f4-2a295298d23c)


### RESULT
The program successfully demonstrates method overriding in Python. The Sparrow and Ostrich classes inherit from the Bird class and override the flight() method. When the method is called, it executes the overridden version based on the object type, showing how method overriding works in object-oriented programming.


