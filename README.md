# Book-Rest-API
# 📚 Book REST API

A simple **REST API** built using **Node.js** and **Express.js** that performs CRUD (Create, Read, Update, Delete) operations on a list of books. The application stores data **in memory**, so no database is required.

---

## 📌 Objective

Build a RESTful API to manage a collection of books using Node.js and Express. The API supports basic CRUD operations and can be tested using tools like **Postman**.

---

## 🚀 Features

- 📖 Get all books
- 🔍 Get a book by ID
- ➕ Add a new book
- ✏️ Update an existing book
- ❌ Delete a book
- 🗂️ In-memory data storage (no database required)
- 📦 JSON request and response handling

---

## 🛠️ Technologies Used

- Node.js
- Express.js
- JavaScript (ES6)
- Postman (for API testing)

---

## 📂 Project Structure

```
Book-REST-API/
│
├── node_modules/
├── package.json
├── package-lock.json
├── server.js
└── README.md
```

---

## 📥 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/book-rest-api.git
```

### 2. Navigate to the project folder

```bash
cd book-rest-api
```

### 3. Install dependencies

```bash
npm install
```

---

## ▶️ Run the Application

Start the server using:

```bash
node server.js
```

or

```bash
npm start
```

The server will start at:

```
http://localhost:3000
```

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Home route |
| GET | `/books` | Get all books |
| GET | `/books/:id` | Get a book by ID |
| POST | `/books` | Add a new book |
| PUT | `/books/:id` | Update a book |
| DELETE | `/books/:id` | Delete a book |

---

## 📥 Sample Request Body (POST)

```json
{
  "title": "Clean Code",
  "author": "Robert C. Martin"
}
```

---

## 📤 Sample Response

```json
{
  "message": "Book Added Successfully",
  "book": {
    "id": 3,
    "title": "Clean Code",
    "author": "Robert C. Martin"
  }
}
```

---

## 🧪 Testing the API

Use **Postman** or any REST API client to test the endpoints.

### Example Requests

### Get All Books

```
GET http://localhost:3000/books
```

### Get Book by ID

```
GET http://localhost:3000/books/1
```

### Add a New Book

```
POST http://localhost:3000/books
```

Body (JSON):

```json
{
  "title": "The Pragmatic Programmer",
  "author": "Andrew Hunt"
}
```

### Update a Book

```
PUT http://localhost:3000/books/1
```

Body (JSON):

```json
{
  "title": "The Alchemist (Updated)"
}
```

### Delete a Book

```
DELETE http://localhost:3000/books/1
```

---

## 📸 Expected Output

Example response from `GET /books`:

```json
[
  {
    "id": 1,
    "title": "The Alchemist",
    "author": "Paulo Coelho"
  },
  {
    "id": 2,
    "title": "Atomic Habits",
    "author": "James Clear"
  }
]
```

---

## 📚 Learning Outcomes

By completing this project, you will learn:

- REST API fundamentals
- Express.js routing
- CRUD operations
- Handling HTTP requests and responses
- JSON data processing
- Building APIs without a database
- Testing APIs using Postman

---

## 🔮 Future Enhancements

- Integrate MongoDB or MySQL
- Add data validation
- Implement authentication (JWT)
- Add pagination and search
- Use environment variables with `.env`
- Improve error handling
- Add unit and integration tests

---

## 👨‍💻 Author

**Harshit Yadav**

---

## 📄 License

This project is developed for educational and learning purposes. You are free to use, modify, and extend it for personal or academic projects.
