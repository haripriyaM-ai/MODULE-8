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

