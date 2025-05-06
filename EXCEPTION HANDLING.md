# Exp.No:17  
## EXCEPTION HANDLING

---

### AIM  
To create a Python program that prompts the user for a list of grades separated by commas, splits the string into individual grades, and uses exception handling to inform the user if the values they entered cannot be converted to integers.

---

### ALGORITHM

1. Begin the program.  
2. Read a string `input_str` from the user using `input()`.  
3. Split the input string using commas (`,`) to create a list of grades.  
4. Use a `try` block to attempt converting each item in the grades list to an integer and store the result in `l1`.  
5. If the conversion is successful, print the list `l1` containing the integer values.  
6. If an error occurs during conversion (for example, if the input is not a valid number), catch the exception and print an error message: `"The grades you entered were in an invalid format."` along with the original grades list.  
7. Terminate the program.

---

### PROGRAM

```
Reg.No:21223060119
Name:Kavindra T G
Add Your Code Here
input_str = input("Enter grades separated by commas: ")
grades = input_str.split(',')

try:
    l1 = [int(grade.strip()) for grade in grades]
    print("Converted grade list:", l1)
except ValueError:
    print("The grades you entered were in an invalid format.")
    print("Original input list:", grades)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/f8a9c89b-0b6c-45c2-aa3f-4308411ac497)

### RESULT
Thus, the python program that prompts the user for a list of grades separated by commas, splits the string into individual grades, and uses exception handling to inform the user if the values they entered cannot be converted to integers has been executed and verified successfully.
