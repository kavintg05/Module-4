# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM

```
#Reg.NO-212223060119
#Name-Kavindra T G
from collections import defaultdict

def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

def character_frequency(file_path):
    with open(file_path, 'r') as file:
        content = file.read()

    d1 = defaultdict(int)
    for ch in content:
        d1[ch] += 1
    return d1

# Example usage:
file_path = "sample.txt"
content = "Hello, World!"

create_file(file_path, content)
freq = character_frequency(file_path)

print("Character frequencies:")
for char, count in freq.items():
    print(f"'{char}': {count}")

```


### OUTPUT
![image](https://github.com/user-attachments/assets/cca054e4-1d5a-43e1-a90a-7b5fff27f03a)


### RESULT
Thus, the python program that reads a file and counts the frequency of each character in it has been executed and verified successfully.
