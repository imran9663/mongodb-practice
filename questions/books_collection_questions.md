
# MongoDB Practice Questions

## General Information
These questions are based on the analysis of a collection containing book documents with fields such as `_id`, `title`, `isbn`, `pageCount`, `publishedDate`, `thumbnailUrl`, `shortDescription`, `longDescription`, `status`, `authors`, and `categories`.

---

## Queries

### Basic
- Write a query to find all books authored by a specific author, such as "Michael Hüttermann".
- Retrieve all books published in or after the year 2010.
- Write a query to find books with `pageCount` greater than 300.
- Find all books categorized as "Java".
- Search for books that contain the word "Flex" in their title.

### Intermediate
- Write a query to find all books where the `status` is "PUBLISH" and the `categories` array includes "Internet".
- Retrieve books with missing or null `thumbnailUrl` fields.
- Write a query to fetch the count of books grouped by their `categories`.
- Retrieve books where the `isbn` field starts with "193".
- Fetch the first 5 books sorted by `publishedDate` in descending order.

### Advanced
- Use an aggregation pipeline to find the total number of pages for books published in each year.
- Write a query to update the `status` of all books with a `pageCount` of 0 to "UNAVAILABLE".
- Use `$regex` to find all books with titles that start with "Android".
- Write an aggregation query to determine the top 3 most frequent authors based on the number of books authored.
- Delete all books published before the year 2000.

---
