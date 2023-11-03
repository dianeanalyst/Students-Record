# Students-Record
Task on creating database and understanding the basics of table formation in data analysis using Structured Query Language.
# Introduction
Working on this task is my first attempt on practicing data analysis using structured query language. This is a tool used to access, process/manipulate data stored in a relational database management system (RDBMS) and  it is called SQL for short. The practice here involved trying my hands on how to create  database and tables from scratch, modifying the tables as necessary and inserting values into the tables.
# Skills demonstrated and activity
In the course of carrying out this task, the activities required that I show some SQL data modification skills and make use of key SQL statements like CREATE, SELECT, ALTER and INSERT INTO which further makes me understand the likely use cases for each statement. A database and three tables were created with named columns and some activities to modify the tables created. The list below shows what was required to fulfil this task.
#
- Create a databse named "Students Record"
#
- Create the following listed tables and column headers in the database created
#
a.  Students Info (Student_ID, Gender, Name, Age, Subject)
#
b.  Health Records (Student ID, Blood Group, Height, Weight)
#
c.  Performance (Student ID, Score, Grade)
#
- The ID has to be unique
- Where a student has no score, it should be '0' by default
- Add a constraint that prevents the ID and Subject from taking null values
- Apply the following modifications to the table
  1. Change column name "Subject" to "Course".
  2. Drop the "Age" column from the Students Info table.
# Solution
I started by creating a database named STUDENT_RECORD using the CREATE statement, then next was to create a table named STUDENTS_INFO commanding sql to create the table in the STUDENT_RECORD database. I did this with the USE statement. Afterwards, I added some values and the column headers to the table using the INSERT INTO statement.

![image](https://github.com/dianeanalyst/Students-Record/assets/120665115/c52d336f-673c-4568-b406-f2195aa02fea)


Same proceure was done to create the other two tables, HEALTH_RECORDS and PERFORMANCE tables. Following the activity which requires modifying STUDENTS_INFO table, I used the code
 EXEC sp_rename 'dbo.STUDENTS_INFO.SUBJECT', 'COURSE', 'COLUMN';  to change the column name "SUBJECT" to "COURSE".

![image](https://github.com/dianeanalyst/Students-Record/assets/120665115/ee3dd932-d71f-46a4-8942-a03513c3ebc6)


![image](https://github.com/dianeanalyst/Students-Record/assets/120665115/af71f153-98ab-4d0d-b07e-891395f20f58)

Using the ALTER TABLE and DROP COLUMN functions, I dropped the column "AGE"from the table.

![image](https://github.com/dianeanalyst/Students-Record/assets/120665115/ce0144c5-e3d5-4c8f-8297-e6931de11362)

# Conclusion
This task and the lessons prior to it have given me hands on experience with navigating through and understanding how the sql console works, some best practices when using this tool and carrying out simple tasks with it. More tasks and projects to expand my sql knowldge and skills will be coming up soonest.

