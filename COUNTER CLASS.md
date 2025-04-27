# Exp.No:30  
## COUNTER CLASS

---

### AIM  
To write a Python program to create a `Counter` class that can increment the value of a counter.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the `Counter` class.**
   - Initialize the `current` variable with 0.
3. **Define the `increment()` method** to increment the value of `current` by 1.
4. **Define the `value()` method** to return the current value of `current`.
5. **Define the `reset()` method** to reset the `current` value back to 0.
6. **Create a `counter` object** of the `Counter` class.
7. **Call the `increment()` method** three times to increment the counter.
8. **Call the `value()` method** and print the result to show the current counter value.
9. **End the program.**

---

### PROGRAM

```
class Counter:
    def __init__(self):
        self.current = 0  # Initializing the counter value to 0

    def increment(self):
        self.current += 1  # Increment the counter by 1

    def value(self):
        return self.current  # Return the current value of the counter

    def reset(self):
        self.current = 0  # Reset the counter to 0

# Create a Counter object
counter = Counter()

# Increment the counter three times
counter.increment()
counter.increment()
counter.increment()

# Print the current value of the counter
print("Current Counter Value:", counter.value())  # Output: 3


```

### OUTPUT

![image](https://github.com/user-attachments/assets/766bc09b-e24a-45bc-b6d3-84bced9c5d6a)


### RESULT
The program successfully implements a Counter class with methods to increment the value, display the current value, and reset the counter. The counter is incremented three times, and the final value is displayed.


