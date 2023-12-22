# Student Directory Table

## Introduction
- This is a simple exercise in Makers Module 3 - Databases
- I used this project to learn how to design and create a schema with two tables.
- `student_directory_two_table_recipe.md` documents my design of the cohorts and students tables
  
## Objectives
- [x] Learn to design and create a schema with two tables and a foreign key.
- [x] Design a two table schema from these user stories.
  - [x] As a coach  
        So I can get to know all students  
        I want to see a list of students' names.
  - [x] As a coach
        So I can get to know all students
        I want to see a list of cohorts' names.
  - [x] As a coach
        So I can get to know all students
        I want to see a list of cohorts' starting dates.
  - [x] As a coach  
        So I can get to know all students  
        I want to see a list of students' cohorts.
        
## Setup

```shell
# Clone the repository to your local machine
; git clone https://github.com/NatalieJClark/student-directory-two-tables.git YOUR_PROJECT_NAME

# Create the database
createdb student_directory;

# Create the tables by running the SQL table file with psql.
psql -h 127.0.0.1 student_directory_2 < students_directory_2.sql

# Enter psql
psql

# Connect to the student_directory database
\c student_directory_2

# View the created tables
SELECT * FROM students
SELECT * FROM cohorts
```
