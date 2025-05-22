## MODULE - 8
# EXP 36 Hackerrank:#  Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.


##  Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.


## Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.



##  PROGRAM:
```
student_marks = {
    'Alice': [85, 90, 88, 92, 80],
    'Bob': [78, 82, 85, 88, 90],
    'Charlie': [90, 91, 92, 93, 94]
}

total_marks = {}

for student in student_marks:
    total_marks[student] = sum(student_marks[student])

topper = max(total_marks, key=total_marks.get)

print(total_marks)
print(topper, total_marks[topper])
```

## OUTPUT
![image](https://github.com/user-attachments/assets/660c8b7d-5faa-4be5-850c-50bec3cb1ab0)

## RESULT
Thus, the program is verified successfully.

---

# EXP 37 Hackerrank :   Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.


## Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.


##  Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.




##  Program
```
def wrap(string, max_width):
    wrapped_lines = []
    for i in range(0, len(string), max_width):
        wrapped_lines.append(string[i:i+max_width])
    return '\n'.join(wrapped_lines)

string = input()
max_width = int(input())
print(wrap(string, max_width))

```
## Output
![image](https://github.com/user-attachments/assets/59a64531-25ee-4452-a4f5-decdc2dbfb34)

## Result
Thus, the program is verified successfully.

---

# EXP 38 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.



##  Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.



##  Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.



## 💻  Program
```
n = int(input())
records = []

for i in range(n):
    name = input()
    grade = float(input())
    records.append([name, grade])

grades = sorted({grade for name, grade in records})
second_lowest = grades[1]

names = [name for name, grade in records if grade == second_lowest]
names.sort()

for name in names:
    print(name)
```

## Output
![image](https://github.com/user-attachments/assets/50920bca-3294-4de3-a44d-ad6571ae106c)

## Result
Thus, the program is verified successfully.

---

# EXP 39 Hackerrank:Runner-Up Score Finder in Python

##  AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.


##  ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**



##  PROGRAM:

```
n = int(input())
scores = list(map(int, input().split()))
unique_scores = list(set(scores))
unique_scores.sort()
print(unique_scores[-2])
```

## OUTPUT
![image](https://github.com/user-attachments/assets/668d58c8-8a9a-4eab-bfaa-f030ed3aacd3)

## RESULT
Thus, the program is verified successfully.

---

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
