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
This project was made with postgreSQL database software. Here's how to install it:
```shell
# Install postgresql (use latest version)
$ brew install postgresql@15

# Make sure the installation directory is on your PATH environment variable
echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc
```
Here's how to run this project:
```shell
# Clone the repository to your local machine
; git clone https://github.com/NatalieJClark/student-directory-two-tables.git YOUR_PROJECT_NAME

# Create the database
createdb student_directory;

# Create the tables by running the SQL table file with psql.
psql -h 127.0.0.1 student_directory_2 < students_directory_2.sql

# Navigate to the student_directory database in psql
psql -h 127.0.0.1 student_directory_2

# View the created tables
SELECT * FROM students;
SELECT * FROM cohorts;
```
