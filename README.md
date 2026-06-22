# Assignment-1
20 Database Questions and Solutions

Assignment 1: Database Setup and Basic Operations
Objective: Set up the database structure for the university course management system and practice basic SQL operations.

Database Setup:
Create a database named University.

Create the following tables with appropriate data types, constraints and keys:
Users (UserId INT PRIMARY KEY, UserName VARCHAR(64) NOT NULL, FirstName VARCHAR(64) NOT NULL, LastName VARCHAR(64) NOT NULL, EmailAddress VARCHAR(128) NOT NULL, PhoneNumber VARCHAR(16) NOT NULL, Role VARCHAR(32) NOT NULL)

Courses (CourseId INT PRIMARY KEY, CourseName VARCHAR(100) NOT NULL, TeacherId INT NULL, StartDate DateTime NOT NULL, EndDate DateTime NOT NULL, SyllabusId NULL)

Assignments (AssignmentId INT PRIMARY KEY, CourseId INT NOT NULL, AssignmentTitle VARCHAR(128) NOT NULL, Description TEXT NULL, Weight float NOT NULL, MaxGrade INT NOT NULL, DueDate DATE NOT NULL)

Comments(CommentId INT PRIMARY KEY, AssignmentId INT NOT NULL, CreatedByUserId not null, CreatedDate DATE TIME NOT NULL, CommentContent TEXT NULL)

Grades (GradeId INT PRIMARY KEY, AssignmentId INT NOT NULL, StudentId INT NOT NULL, Grade INT NULL)

Syllabus (SyllabusId INT PRIMARY KEY, Description TEXT NULL)

An email address must be unique in the user table.

 

Requirements:

Write SQL statements to INSERT data for all the interns into the user table with Role ‘Student’

Write SQL statements to INSERT data for Sami, Feryal into the user table with Role ‘Teacher’

Write SQL statements to INSERT data for SQL, C#, Entity Framework, Web API and React Courses.

Write SQL Statements to INSERT at least 5 Assignments for each Course with random due dates (past & future).

Write SQL Statements to INSERT at least 10 comments for random assignments.

Write SQL Statement to INSERT random grades for all students for every assignment.

Write SQL Statement to INSERT Syllabus for each Course.

Write a SELECT query to list all courses.

Write a SELECT query to find all assignments for a specific course.

Write a SELECT query to find all students (users with the role 'Student').

Write an UPDATE statement to change a student's role.

Write a DELETE statement to remove a specific comment.

Write a query to list all students along with their grades for a specific course.

Write a query to calculate the average grade for each course.

Write a query to list all courses with their respective syllabuses.

Write a query to find all comments for a specific course.

Create a stored procedure to add a new student.

Create a stored procedure to add a new Assignment. Make sure the course assignments weights don’t go above 100.

Calculate function to calculate the Student Grade in a Course. Return ‘A', 'B’, etc…

Create a function to calculate the GPA of a student.
