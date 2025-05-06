# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

---

### AIM  
To write a Python program to perform addition and division operations using a class. The class should be named `Saveetha`, and the function names should be `setvalues` (to set `a` and `b` values), `add`, and `div`. The program should handle the following cases:  
- `choice 1` → Perform addition  
- `choice 2` → Perform division  
- `choice 0` → Exit  
- For other choices, print 'Invalid choice'

---

### ALGORITHM

1. Begin the program.  
2. Create a class `Saveetha`.  
3. Define the following methods inside the `Saveetha` class:  
   - `__init__(self)`: Initializes `a` and `b` to zero.  
   - `setvalues(self, a, b)`: Sets the values of `a` and `b`.  
   - `add(self)`: Performs the addition operation.  
   - `div(self)`: Performs the division operation. If `b` is zero, returns an error message for division by zero.  
4. Create a `main()` function.  
5. Take input from the user for the values of `a` and `b` using `setvalues(a, b)` method.  
6. Use a `while True` loop to repeatedly ask the user for a choice:  
   - If the choice is 1, call the `add()` method and print the result.  
   - If the choice is 2, call the `div()` method and print the result. Handle division by zero.  
   - If the choice is 0, print "Exiting!" and exit the loop.  
   - If the choice is not 1, 2, or 0, print "Invalid choice".  
7. Terminate the program.

---

### PROGRAM

```
#Reg.NO-212223060119
#Name-Kavindra T G
class Saveetha:
    def __init__(self):
        self.a = 0
        self.b = 0

    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def add(self):
        return self.a + self.b

    def div(self):
        if self.b == 0:
            return "Error: Division by zero is not allowed."
        return self.a / self.b

def main():
    obj = Saveetha()
    a = int(input("Enter value of a: "))
    b = int(input("Enter value of b: "))
    obj.setvalues(a, b)

    while True:
        print("\nMenu:")
        print("1. Addition")
        print("2. Division")
        print("0. Exit")
        choice = int(input("Enter your choice: "))

        if choice == 1:
            print("Result of addition:", obj.add())
        elif choice == 2:
            result = obj.div()
            print("Result of division:", result)
        elif choice == 0:
            print("Exiting!")
            break
        else:
            print("Invalid choice")

main()




```

### OUTPUT
![image](https://github.com/user-attachments/assets/350ca47a-32ed-4ba6-94f6-963de66b652c)

### RESULT
Thus,the Python program using the Saveetha class successfully performed addition and division based on user choice.
