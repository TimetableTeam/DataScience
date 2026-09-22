# Tanseek v2 data package

This package adds students, course registration, and individual Lecture/Practical section assignment.

## Decisions represented

- Every offered course has exactly two requirement types: `LECTURE` and `PRACTICAL`.
- A type may have multiple sections; for example one lecture stream and two practical streams.
- `REGISTRATION_OFFICER` registers students in courses.
- `DEPARTMENT_COORDINATOR` assigns registered students to one Lecture and one Practical section.
- `SCHEDULER` assigns section times and rooms.
- `student_section_enrollments` is authoritative for the personal timetable.
- Every student has a linked `STUDENT` account for read-only login.
- Student Groups are optional organisational cohorts used for bulk assignment.
- No prerequisites, credit-hour limits, GPA rules, or level restrictions are invented because the academic bylaws are not available.

## Files

- `Tanseek_PostgreSQL_Schema_v2.sql`: complete PostgreSQL baseline.
- `Tanseek_ERD_v2.md`: one Mermaid ERD plus entity definitions.
- `Tanseek_Data_v2.xlsx`: all sample tables in one workbook.
- `csv/`: the same sample data as individual CSV files.
- `constraint_test_cases.csv`: proposals with expected validation outcomes.

All people and identifiers in the sample data are synthetic.
