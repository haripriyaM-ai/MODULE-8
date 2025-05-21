# EXP 40 Hackerrank:Python Program to Check if a String Ends with a Numeric Digit

This Python program checks whether the last character of a given input string is a **numeric digit (0–9)**.



##  Aim

To write a Python program that checks if a given string ends with a number using Python's built-in string methods.



##  Algorithm

1. **Start the program.**
2. **Input** a string from the user.
3. **Access** the last character using indexing (`string[-1]`).
4. **Check** if the last character is a digit using the `.isdigit()` method.
5. **If true**, print that the string ends with a number.
6. **Else**, print that the string does not end with a number.
7. **End the program.**



##   Program
```
string = input()
if string[-1].isdigit():
    print("String ends with a number")
else:
    print("String does not end with a number")

```
## Output
![image](https://github.com/user-attachments/assets/402c7074-c2a7-40dd-a7d3-16605eedf008)

## Result
Thus, the program is verified successfully.
