# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

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

---

## 💻 PROGRAM:
```
m1,m2,m3=int(input()),int(input()),int(input())
total=m1+m2+m3;
percentage=(total/300)*100
print("Total marks obtained is {} and the percentage obtained is {}".format(total,percentage))
```
## OUTPUt
![442607051-ba7a3960-ddb6-422b-9432-ad47c981b1ad](https://github.com/user-attachments/assets/49315323-903d-4723-a732-dfe051e6242e)


## RESULT
Program is verified.

# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
```
def wrap(string, max_width):
    wrapped_lines = []
    for i in range(0, len(string), max_width):
        wrapped_lines.append(string[i:i+max_width])
    return '\n'.join(wrapped_lines)

# Example usage
text = input("Enter a long string: ")
width = int(input("Enter max width: "))
print("\nWrapped Text:\n")
print(wrap(text, width))
```
## Sample Output
![442607353-2b4d8e9d-9a10-442f-a211-8711293d4f67](https://github.com/user-attachments/assets/049f74c2-5f8d-4664-8585-655b7da56e31)

## Result
Program is verified successfully.

# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
```
n = int(input("Enter the number of students: "))
students = []

# Read student names and grades
for _ in range(n):
    name = input("Enter student's name: ")
    grade = float(input("Enter student's grade: "))
    students.append([name, grade])

# Extract and sort the grades
grades = sorted(set([student[1] for student in students]))

# Identify the second lowest grade
second_lowest_grade = grades[1]

# Collect names of students with the second lowest grade
second_lowest_students = sorted([student[0] for student in students if student[1] == second_lowest_grade])

# Print the sorted names
for name in second_lowest_students:
    print(name)
```
## Output
![442608076-a0bb7bf2-9dc0-4280-8749-2104222d4b5a](https://github.com/user-attachments/assets/82d01325-1f09-46a0-9c70-8dc14b1e1e83)

## Result
Thus,the program is executed successfully

