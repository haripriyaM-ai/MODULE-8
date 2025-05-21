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
