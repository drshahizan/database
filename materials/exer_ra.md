
<a href="https://github.com/drshahizan/database/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/database" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/database/network/members"><img src="https://img.shields.io/github/forks/drshahizan/database" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/database/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/database" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/database/issues"><img src="https://img.shields.io/github/issues/drshahizan/database" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/database/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/database?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdatabase&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

# Relational Algebra — Practice Set (Malaysia Context)

## Mini Dataset (use these schemas throughout)

**Student(StudentID, Name, Gender, State, ProgramID, YearOfStudy, CGPA)**

```
S1001, "Nur Aisyah",  F, "Johor",   P10, 2, 3.82
S1002, "Ahmad Firdaus", M, "Selangor", P20, 3, 3.10
S1003, "Tan Wei Ling", F, "Johor",   P10, 1, 3.67
S1004, "Aina Sofea",   F, "Penang",  P30, 2, 3.45
S1005, "Syafiq Razif", M, "Johor",   P10, 4, 3.25
```

**Program(ProgramID, ProgramName, Faculty)**

```
P10, "Bachelor of Computer Science", "Faculty of Computing"
P20, "Bachelor of Information Systems", "Faculty of Computing"
P30, "Bachelor of Electrical Engineering", "Faculty of Engineering"
```

**Course(CourseID, CourseName, CreditHour, ProgramID)**

```
C201, "Programming Technique I",   3, P10
C202, "Programming Technique II",  3, P10
C203, "Database Systems",          3, P20
C301, "Circuit Theory",            4, P30
```

**Enrollment(StudentID, CourseID, Grade)**

```
S1001, C201, "A-"
S1001, C202, "A"
S1003, C201, "B+"
S1003, C202, "A-"
S1005, C202, "B"
S1002, C203, "A-"
S1004, C301, "B+"
```

## Part A — Core Operations

1. **Selection (σ)**
   Write a relational algebra expression to list **Johor** students with **CGPA ≥ 3.60**.

2. **Projection (π)**
   Return only **Name** and **CGPA** of all students.

3. **Union (∪)**
   Suppose `JohorStudents` and `SelangorStudents` are derived from `Student`.
   Write a union expression that lists **all students from Johor or Selangor** without duplicates.

4. **Set Difference (−)**
   Using `Enrollment`, list **students who have taken C202** but **not C201**.

5. **Cartesian Product (×) then Selection**
   Produce all **valid Lecturer–Course** pairs if we had `Lecturer(LecturerID, LecturerName, Faculty)` and wanted to **pair only lecturers in the same faculty as the course’s program**.
   (Write the general RA using symbols; you don’t need concrete tuples.)

6. **Rename (ρ)**
   Rename `Student` to `Pelajar` and attributes to **(ID, Nama, Jantina, Negeri, Program, Tahun, PNGK)**.

7. **Natural/Theta Join (⋈)**
   Join `Student` and `Program` to show each student with their **ProgramName** and **Faculty**.

8. **Join Chain**
   Retrieve **StudentID, Name, CourseName** for **all enrollments** (join `Student`, `Enrollment`, `Course`).

## Part B — Malaysia-Flavoured Analytics

9. **Top course among Johor female students**
   Using RA, return the **CourseName(s)** most frequently taken by **female students from Johor** in the sample data.

10. **Average CGPA by Faculty**
    Using RA + aggregation notation (γ), compute the **average CGPA** of students **grouped by Faculty** (via join to `Program`).
    *(If your course hasn’t covered extended algebra/aggregation, write the pipeline up to the grouped relation and describe the final step.)*

## Part C — UTM Case Study Task

**Goal:** Find **names of female students** from the **Faculty of Computing** who are **enrolled in “Programming Technique II.”**

1. Write the **relational algebra** pipeline.
2. Provide the **SQL equivalent**.
3. Using the sample tuples, **list the resulting names**.

## Bonus Challenges (for fast finishers)

B1) **Prerequisite check (set logic):**
Students who have **C202** must also have **C201**. Using RA, produce the set of **students violating** this rule.

B2) **Cross-faculty enrollment:**
List students whose **Program Faculty** is **different** from the **Faculty of the course** they took (via `Course.ProgramID → Program.Faculty`).


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/HPDP/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)




