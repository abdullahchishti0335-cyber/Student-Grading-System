# 🎓 Student Grading System 🐍

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-blue)]()

A beginner-friendly **Python project** that calculates student grades based on their marks.  
It uses **functions** for clean code, supports **multiple students**, and includes **input validation** for reliability.

---

## 🚀 Features
✅ Accepts multiple students  
✅ Validates marks range (0–520)  
✅ Automatically assigns grades (A+ to F)  
✅ Simple and beginner-friendly structure  
✅ Written using clean, functional Python code  

---

## 🧮 Grading Criteria

| Marks Range | Grade |
|--------------|--------|
| 500 – 520    | A+     |
| 450 – 499    | A      |
| 400 – 449    | B+     |
| 350 – 399    | B      |
| 300 – 349    | C     |
| 250 – 299    | D      |
| Below 250    | F      |

---

## 🧩 Example Code

```python
def student_grades(marks):
    if marks < 0 or marks > 520:
        return "Invalid Marks, Write a value between 0 to 520"
    elif marks >= 500:
        return "A+"
    elif marks >= 450:
        return "A"
    elif marks >= 400:
        return "B+"
    elif marks >= 350:
        return "B"
    elif marks >= 300:
        return "C"
    elif marks >= 250:
        return "D"
    else:
        return "F"

students = []
num_students = int(input("Enter the Total Number of Students: "))

for i in range(num_students):
    print(f"\n Student {i + 1}:")
    name = input("Enter Student Name: ")
    marks = int(input("Enter Student Marks (0-520): "))
    grade = student_grades(marks)

    students.append({
        "name": name, "marks": marks, "grade": grade
    })

print("\n----Student Grades Result----")
for result in students:
    print(f"Name: {result['name']}, Marks: {result['marks']}, Grade: {result['grade']}")
 ```


## 💻 How to Run

1. Make sure **Python 3.x** is installed: [Python Download](https://www.python.org/downloads/)  
2. Install **Jupyter Notebook** (if not installed):
   ```bash
   pip install notebook

3. Open the project folder in a terminal or command prompt.
4. Start Jupyter Notebook:
    ```bash
    jupyter notebook

5. Click on student_grading_system.ipynb to open it.
6. Run the cells in order (Shift + Enter) and follow the prompts:
    *Enter the total number of students*
    *Enter each student’s name and marks*

## 🧰 Requirements

1. *Python 3.x*
2. *Jupyter Notebook (optional, but recommended for running .ipynb files)*

## 🧑‍💻 Author

**Abdullah Rajpoot**
🌐 GitHub: https://github.com/abdullahchishti0335-cyber
