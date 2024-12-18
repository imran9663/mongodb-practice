
# MongoDB Practice Questions

## CRUD Operations
### Basic
- Write a query to insert a new document into the collection.
- Retrieve all documents where the `age` is greater than 25.
- Write a query to update the `is_active` field to `true` for all documents where `age` is less than 30.
- Delete all documents where the `skills` array includes "SQL".

### Intermediate
- Update the `years_worked` field of the first employment history record to 5 for all employees who have "React" as a skill.
- Write a query to add a new hobby "Hiking" to all documents where `hobbies` does not include "Traveling".
- Remove the last employment history entry for employees who have worked in more than 2 companies.
- Replace the entire `address` field for a user with a specific `_id`.

## Query Operators
### Basic
- Retrieve documents where `age` is between 20 and 40 using `$gte` and `$lte`.
- Find all documents where `hobbies` include both "Gaming" and "Reading".
- Write a query to retrieve documents where `skills` contains "Python" but not "JavaScript".

### Intermediate
- Retrieve documents where `education.year` is greater than 2010.
- Write a query to find all employees who worked as a "Manager" in their employment history.
- Use `$regex` to find documents where the `name` starts with "J".

## Aggregation
### Basic
- Use `$group` to count the number of employees in each city.
- Write a query to calculate the average `age` of all employees.

### Advanced
- Use `$unwind` and `$group` to count the number of unique skills across all documents.
- Write an aggregation pipeline to find the top 3 universities attended by employees.
- Calculate the total `years_worked` for all employees grouped by their state.

## Indexing
### Basic
- Create an index on the `age` field.
- Write a query to find all employees sorted by `name` in ascending order.

### Advanced
- Create a compound index on `skills` and `city`. Test it with a query.
- Use `$hint` to force a specific index during a query execution.

---
