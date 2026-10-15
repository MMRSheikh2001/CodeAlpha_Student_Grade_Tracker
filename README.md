# Student Grade Tracker

A desktop application built with **Java Swing** for entering student scores and viewing basic grade statistics. Student data is stored in memory using an `ArrayList`.

Created as a Java programming task for CodeAlpha.

## Features

- Add a student by name and score (0–100)
- Input validation for empty fields, non-numeric scores and out-of-range scores
- Table listing every student with serial number, name, score and letter grade
- Class statistics shown on the form:
  - Average score
  - Highest score, with the student's name
  - Lowest score, with the student's name
- Delete a selected student from the table
- Clicking a table row loads that student's name and score into the input fields
- Reset button to clear the input fields

## Grading Scale

| Score | Grade |
|-------|-------|
| 90 and above | A |
| 80 – 89 | B |
| 70 – 79 | C |
| 60 – 69 | D |
| Below 60 | F |

## Technologies

- Java (JDK 8 or later)
- Swing (`JFrame`, `JTable`, `DefaultTableModel`, `JOptionPane`)
- `ArrayList` for data storage
- NetBeans (Ant project, GUI built with the NetBeans Form Editor)

## Project Structure

```
Student_Grade_Tracker/
└── src/student_grade_tracker/
    ├── Student.java            # Model: name, score, letter grade
    ├── StudentGradeForm.java   # Swing GUI and event handling
    └── Student_Grade_Tracker.java
```

- `Student` holds a student's name and score and calculates the letter grade.
- `StudentGradeForm` keeps a `List<Student>`, refreshes the table from it and calculates the average, highest and lowest scores.

## How to Run

**Using NetBeans**
1. Clone the repository:
   ```
   git clone https://github.com/MMRSheikh2001/CodeAlpha_Student_Grade_Tracker.git
   ```
2. Open the `Student_Grade_Tracker` folder as a project in NetBeans.
3. Open `StudentGradeForm.java` and choose **Run File** (Shift + F6).

## Usage

1. Enter a student's name and score, then click **Submit**.
2. The student appears in the table and the statistics update.
3. To remove a student, select their row and click **Delete Student**.
4. Click **Reset** to clear the name and score fields.

## Limitations

- Data is kept in memory only and is lost when the application is closed.
- Each student has a single score.

## Author

MD Mahbubur Rahman Sheikh — [@MMRSheikh2001](https://github.com/MMRSheikh2001)