# MongoDB Practice Repository

Welcome to the **MongoDB Practice Repository**! This repository is designed to help you master MongoDB by practicing CRUD operations, aggregation pipelines, indexing, array operations, and more. It includes realistic datasets, example queries, and problem-based exercises.

---

## 📂 Repository Structure

- **`sample_data/`**  
  Contains JSON datasets for practice, such as employee details, books, student records, and more.  
  - `employees.json`: Dataset with over 100 documents, including nested documents and arrays.
  - `books.json`: These questions are based on the analysis of a collection containing book documents with fields such as `_id`, `title`, `isbn`, `pageCount`, `publishedDate`, `thumbnailUrl`, `shortDescription`, `longDescription`, `status`, `authors`, and `categories`..

- **`questions/`**  
  Problem-based MongoDB practice questions in Markdown format.  


---

## 📖 Topics Covered

### 1. CRUD Operations  
Learn to insert, update, delete, and retrieve data from collections with practical exercises.

### 2. Query Operators  
Master MongoDB operators like `$eq`, `$ne`, `$gte`, `$lte`, `$in`, `$regex`, and more.

### 3. Array Operations  
Understand how to work with arrays using `$push`, `$pop`, `$addToSet`, `$unwind`, and `$elemMatch`.

### 4. Aggregation Pipelines  
Practice building complex aggregation queries using `$match`, `$group`, `$project`, `$lookup`, and `$bucket`.

### 5. Indexing  
Learn to optimize query performance by creating single-field and compound indexes.

---

## 🚀 How to Use

### Clone the Repository
```bash
git clone https://github.com/imran9663/mongodb-practice.git
cd mongodb-practice
```
---
## 🚀 Load the Data into MongoDB

### Steps to Import Data:
1. Start your MongoDB server.

2. Use the `mongoimport` tool to load the dataset into your MongoDB instance:

   ```
   mongoimport --db practice_db --collection employees --file sample_data/books.json --jsonArray
   ```
3. Verify the data has been imported correctly:

    ```
    use practice_db
    db.employees.find().pretty()
    ```


---
## 📝 Exercises

### CRUD Operations
- Insert new documents into the collection.
- Update documents using `$set`, `$unset`, and `$rename`.
- Delete specific documents using `$match`.

### Query Operators
- Retrieve documents with complex filter conditions.
- Perform text searches with `$regex`.

### Aggregation Pipelines
- Group documents by a specific field.
- Create custom fields using `$addFields`.
- Perform lookups to join collections.

### Indexing
- Create indexes and analyze query performance with `$explain`.
- Use compound indexes for multi-field queries.

---
## 🤝 Contributing

We welcome contributions! Feel free to:

- Add more datasets to the `sample_data/` folder.
- Submit new practice questions or solutions.
- Report bugs or suggest improvements.

### Steps to Contribute:
1. Fork the repository.
2. Create a new branch: ```bash git checkout -b feature-name```
3. Commit your changes: `git commit -m "Add new feature"`.
4. Push to your branch: `git push origin feature-name`.
5. Open a pull request.
---
## 📬 Contact
If you have any questions or feedback, feel free to reach out:

- Author: Imran Pasha
- Portfolio: [imranpashai.netlify.app](https://imranpashai.netlify.app)
- GitHub: [imran9663](https://github.com/imran9663)
