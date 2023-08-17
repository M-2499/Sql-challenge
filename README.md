# Sql-challenge

Employee Database and Data Analysis: 

Welcome to the Employee Database and Data Analysis repository. This repository contains SQL scripts that define a database schema and perform various data analysis tasks on it. The database schema includes tables for employee information, titles, departments, salaries, and more. The provided SQL queries allow you to extract valuable insights from this database.

Creating Tables
The database structure is established using SQL Data Definition Language (DDL) statements, which define the tables to hold various types of information. Each table corresponds to a specific aspect of the organizational data. Here's a brief summary of the table creation process:

titles Table
The titles table is designed to store employee titles. It contains columns for title_id (unique identifier for titles) and title (the actual title). The title_id column is designated as the primary key to ensure uniqueness.

employees Table
The employees table is where detailed employee information is stored. Columns include emp_no (unique employee identifier), emp_title_id (foreign key referencing titles), birth_date, first_name, last_name, sex, and hire_date. The emp_no column is the primary key, and emp_title_id establishes a link to the titles table.

departments Table
The departments table holds department-related data. It consists of columns for dept_no (unique department identifier) and dept_name. The dept_no column serves as the primary key.

dept_manager Table
The dept_manager table tracks department managers. It includes columns for dept_no (foreign key referencing departments), emp_no (foreign key referencing employees), and both columns together form the primary key.

dept_emp Table
The dept_emp table records the relationship between employees and departments. Columns emp_no and dept_no (both foreign keys) establish these associations. Together, they form the primary key.

salaries Table
The salaries table holds information about employee salaries. Columns include emp_no (foreign key referencing employees) and salary. The emp_no column is part of the primary key, and it references the employees table.

These tables are the foundation of the database, organizing data into meaningful categories for efficient storage and retrieval.



Data Analysis Queries

--The repository includes a set of SQL queries designed to analyze the employee database and answer various questions. These queries provide insights into -----------different aspects of the organization:

--List Employee Details and Salary: Retrieve employee number, last name, first name, sex, and salary of each employee.

--Hire Date in 1986: List first name, last name, and hire date for employees hired in the year 1986.

--Department Managers: Display the department number, department name, employee number, last name, and first name of department managers.

--Employee Department Association: Show department number, employee number, last name, first name, and department name of employees.

--Specific Employee Query: List first name, last name, and sex of employees named Hercules with last names starting with "B".

--Employees in Sales Department: Display employee number, last name, and first name of employees in the Sales department.

--Employees in Sales and Development Departments: List employee number, last name, first name, and department name for employees in the Sales and Development --------departments.
--Last Name Frequency: Provide a frequency count of employee last names, ordered in descending order by frequency.



Getting Started

To explore the database schema and run the data analysis queries, follow these steps:

Database Setup: Set up a database management system (DBMS) such as MySQL or PostgreSQL and execute the provided CREATE TABLE statements to create the tables.
Data Import: Populate the tables with sample data using INSERT INTO statements.
Data Analysis: Run the data analysis queries to extract insights from the database.


Feel free to modify the queries or expand the database with additional data to further explore its capabilities.

Happy exploring and analyzing!

