# 📝 FastAPI Blog Project

A modern Blog Management System built with **FastAPI**, **SQLAlchemy**, **Jinja2**, **Bootstrap**, and **JavaScript**. The application allows users to create, view, edit, and delete blog posts through a clean web interface while following a well-structured FastAPI project architecture.

---

## 📌 Features

- Create blog posts
- View all blog posts
- Update existing posts
- Delete blog posts
- Responsive Bootstrap UI
- RESTful API
- Server-side rendering using Jinja2
- SQLAlchemy ORM
- Form validation
- Modular project structure
- Reusable JavaScript utility functions
- Clean and maintainable codebase

---

## 🛠 Tech Stack

### Backend

- FastAPI
- SQLAlchemy
- Pydantic
- Uvicorn

### Frontend

- HTML5
- CSS3
- Bootstrap 5
- JavaScript (ES6)

### Database

- SQLite

---

## 📁 Project Structure

```
blog-project/
│
├── app/
│   ├── routers/
│   ├── models/
│   ├── schemas/
│   ├── database.py
│   ├── config.py
│   └── main.py
│
├── static/
│   ├── css/
│   ├── js/
│   │   ├── utils.js
│   │   ├── blog.js
│   │   └── ...
│   └── images/
│
├── templates/
│
├── requirements.txt
├── README.md
└── .env
```

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd blog-project
```

### 2. Create Virtual Environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
uvicorn app.main:app --reload
```

---

## 🌐 Open in Browser

Application

```
http://127.0.0.1:8000
```

Swagger Documentation

```
http://127.0.0.1:8000/docs
```

ReDoc Documentation

```
http://127.0.0.1:8000/redoc
```

---

## 📖 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Home Page |
| GET | `/posts` | Get all posts |
| GET | `/posts/{id}` | Get single post |
| POST | `/posts` | Create new post |
| PUT | `/posts/{id}` | Update post |
| DELETE | `/posts/{id}` | Delete post |

> Endpoint names may vary depending on your router configuration.

---

## 💻 Frontend

The frontend is built using:

- HTML5
- Bootstrap 5
- Vanilla JavaScript

JavaScript communicates with the FastAPI backend using the **Fetch API**.

Example:

```javascript
fetch("/posts")
    .then(response => response.json())
    .then(data => console.log(data));
```

---

## 📂 JavaScript Utilities

The project includes reusable helper functions inside:

```
static/js/utils.js
```

These utilities handle common tasks such as:

- Showing Bootstrap modals
- Hiding Bootstrap modals
- Formatting API error messages

Keeping reusable code in one file avoids duplication and improves maintainability.

---

## 🗄 Database

The project uses **SQLite** with **SQLAlchemy ORM**.

Benefits:

- Easy setup
- Lightweight
- Beginner friendly
- Supports ORM relationships
- Easy migration to PostgreSQL or MySQL

---

## 🏗 Project Workflow

```
User
   │
   ▼
Frontend (HTML + JS)
   │
Fetch API
   │
   ▼
FastAPI
   │
SQLAlchemy
   │
SQLite Database
   │
   ▼
JSON Response
   │
Frontend Updates UI
```

---

## 📚 Learning Objectives

This project demonstrates:

- FastAPI fundamentals
- API development
- CRUD operations
- SQLAlchemy ORM
- Pydantic validation
- Template rendering with Jinja2
- JavaScript Fetch API
- Bootstrap integration
- Clean project architecture
- Separation of concerns

---

## 🔮 Future Improvements

- User Authentication
- JWT Authorization
- User Roles
- Rich Text Editor
- Categories
- Tags
- Search
- Comments
- Likes
- Pagination
- Image Upload
- Email Verification
- Docker Support
- PostgreSQL Deployment
- Unit Testing
- CI/CD Pipeline

---

## 👨‍💻 Author

**Manank Pandya**

- B.Tech Computer Engineering
- Python & FastAPI Developer
- Passionate about Backend Development

---

## 📄 License

This project is created for educational and learning purposes.
