
# MongoDB Problem-Based Practice Questions

## Basic Questions
1. **Find all books by a specific author.**  
   Write a query to find all books authored by "Michael Hüttermann".

2. **Find books by category.**  
   Write a query to fetch all books that belong to the "Software Engineering" category.

3. **Find recently published books.**  
   Write a query to find all books published after January 1, 2015.

4. **Search by title keyword.**  
   Write a query to find all books whose title contains the word "Agile".

5. **Filter by status.**  
   Write a query to find all books with the status "PUBLISH".

## Intermediate Questions
1. **Find books with a minimum page count.**  
   Write a query to find all books with a page count greater than 300.

2. **Combine multiple filters.**  
   Write a query to find all books published after January 1, 2010, authored by "Michael Hüttermann", and categorized under "Software Engineering".

3. **Pagination.**  
   Write a query to fetch the first 10 books sorted by their `publishedDate` in descending order.

4. **Find books with multiple authors.**  
   Write a query to fetch all books that have more than one author.

5. **Find books with missing information.**  
   Write a query to find all books where the `pageCount` is equal to 0.

## Advanced Questions
1. **Aggregate books by category.**  
   Write an aggregation query to count the number of books in each category.

2. **Group by publication year.**  
   Write an aggregation query to group books by the year they were published and count the number of books published in each year.

3. **Find books with specific ISBN patterns.**  
   Write a query to find all books where the `isbn` starts with "193".

4. **Update book details.**  
   Write a query to update the `status` of all books authored by "Michael Hüttermann" to "ARCHIVED".

5. **Delete outdated books.**  
   Write a query to delete all books published before January 1, 2000.

6. **Search in nested arrays.**  
   Write a query to find all books with the category "Agile" in their `categories` array.

7. **Top categories by book count.**  
   Write an aggregation query to find the top 3 categories with the most books.

8. **Fetch books without specific fields.**  
   Write a query to fetch all books where the `thumbnailUrl` field is missing or null.

---

### Notes:
- Use appropriate MongoDB operators like `$gte`, `$regex`, `$exists`, `$unwind`, `$group`, and `$sort` where applicable.
- Ensure efficient indexing for optimal query performance.
