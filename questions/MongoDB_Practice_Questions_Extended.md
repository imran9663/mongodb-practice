
# MongoDB Practice Questions for CRUD, Aggregation, and More

## General Information
This set of questions is designed to help you practice MongoDB operations on a dataset of employees. Each document represents an employee with fields like `_id`, `name`, `age`, `address`, `contactNumbers`, `skills`, `projects`, `isActive`, `salary`, and `dateOfJoining`.

---

## CRUD Operations

### Basic
- Retrieve all employees aged above 30.
- Find employees with the skill "Python".
- Insert a new employee document with at least 3 skills and 2 projects.
- Update the `isActive` status to `False` for employees whose salary is less than 50,000.
- Delete employees who have not worked on any projects.

### Intermediate
- Update the `address.city` field for all employees in the "California" state to "San Francisco".
- Add a new skill "Kubernetes" to employees who already know "Docker".
- Remove the contact number of employees who have more than 2 contact numbers.
- Retrieve employees who joined the company after January 1, 2020, sorted by `salary` in descending order.
- Fetch employees working on "In Progress" projects.

### Advanced
- Replace the address field with only `city` and `country` for employees who live in "New York".
- Use `$regex` to find employees whose names start with "John".
- Write an aggregation query to group employees by their `skills` and count the number of employees for each skill.
- Create an index on the `salary` field and demonstrate its effect on query performance.
- Use `$lookup` to combine employee data with another collection of departments, showing employees and their respective departments.

## Array Operations

### Basic
- Retrieve employees with more than 3 skills.
- Find employees working on projects where the status is "Completed".

### Intermediate
- Update the `projects` array by adding a new project to employees with no "In Progress" projects.
- Remove all projects with the status "On Hold" for employees.

### Advanced
- Write an aggregation pipeline to count the total number of projects grouped by their `status`.
- Flatten the `projects` array to retrieve a list of all project titles across all employees.

## Aggregation Pipeline

### Basic  
- Use the `$match` stage to filter documents where `age` is greater than 30.  
- Use the `$project` stage to include only the `name` and `skills` fields in the output.  
- Use `$group` to count the total number of documents in the collection.  
- Use `$sort` to sort documents by `age` in descending order.  
- Use `$limit` to retrieve the top 5 oldest employees.  

### Intermediate  
- Combine `$match` and `$group` to count the number of employees in each city.  
- Use `$unwind` and `$group` to find the number of employees with each unique skill.  
- Use `$project` to create a new field `is_senior` that is `true` if `age` is above 40 and `false` otherwise.  
- Combine `$unwind`, `$group`, and `$avg` to calculate the average `years_worked` for all employees.  
- Use `$match` and `$count` to find the number of employees with "Gaming" as a hobby.  

### Advanced  
- Write a pipeline to find the top 3 most common hobbies across all employees.  
- Use `$bucket` to group employees into age ranges (e.g., 18-25, 26-35, 36-50).  
- Use `$lookup` to join the current collection with another collection (e.g., `departments`) to retrieve department details for each employee.  
- Combine `$addFields` and `$project` to calculate the total years of education for each employee and include it as a new field.  
- Write a pipeline to find the top 5 companies based on the total `years_worked` by employees for those companies.  

## Indexing and Optimization

### Basic
- Create an index on the `isActive` field to optimize queries for active employees.

### Intermediate
- Explain how to use compound indexes for fields like `skills` and `salary`.

### Advanced
- Write a query to demonstrate the use of `$explain` for analyzing query performance.
