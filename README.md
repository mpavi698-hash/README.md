# 🎓 Student Management System API

A RESTful API built with **Python**, **FastAPI**, and **SQLite** to manage student information, subjects, marks, and reports.

---

## 📖 About the Project

The Student Management System API is designed to help schools and coaching centers manage student records efficiently. It provides endpoints for creating, updating, deleting, and retrieving student data. It also supports managing subjects, recording marks, and generating useful reports such as toppers and rank lists.

---

## ✨ Features

- ✅ Add new students
- ✅ View all students
- ✅ Update student information
- ✅ Delete students
- ✅ Add subjects
- ✅ Store student marks
- ✅ Search students by name
- ✅ Search students by city
- ✅ Sort students by name or age
- ✅ Generate student report cards
- ✅ Find class topper
- ✅ Find failed students
- ✅ Generate rank list

---

## 🛠️ Technologies Used

- Python 3
- FastAPI
- SQLite
- Uvicorn
- Pydantic

---

## 📁 Project Structure

```
student-management-api/
│
├── main.py
├── database.py
├── models.py
├── schemas.py
├── crud.py
├── database.db
├── requirements.txt
└── README.md
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/student-management-api.git
```

### 2. Go to the project folder

```bash
cd student-management-api
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
uvicorn main:app --reload
```

The server will start at:

```
http://127.0.0.1:8000
```

---

## 📚 API Documentation

Swagger UI

```
http://127.0.0.1:8000/docs
```

ReDoc

```
http://127.0.0.1:8000/redoc
```

---

## 📌 API Endpoints

### Students

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /students | Create a student |
| GET | /students | Get all students |
| GET | /students/{id} | Get student by ID |
| PUT | /students/{id} | Update student |
| DELETE | /students/{id} | Delete student |

### Subjects

| Method | Endpoint |
|--------|----------|
| POST | /subjects |
| GET | /subjects |

### Marks

| Method | Endpoint |
|--------|----------|
| POST | /marks |
| GET | /marks |

### Reports

| Method | Endpoint |
|--------|----------|
| GET | /report/student/{id} |
| GET | /report/topper |
| GET | /report/failed |
| GET | /report/rank-list |

---

## 📥 Example Student Request

```json
{
    "name": "Pavithra",
    "age": 20,
    "gender": "Female",
    "city": "Chennai"
}
```

---

## 📤 Example Response

```json
{
    "id": 1,
    "name": "Pavithra",
    "age": 20,
    "gender": "Female",
    "city": "Chennai"
}
```

---

## 🔍 Validation Rules

- Name cannot be empty.
- Age must be between 15 and 25.
- Gender must be Male, Female, or Other.
- Marks must be between 0 and 100.
- Student and Subject must exist before adding marks.

---

## 📈 Future Improvements

- JWT Authentication
- User Login
- Role-Based Access Control
- Pagination
- Export Reports to Excel/PDF
- Docker Support
- Unit Testing
- Deployment to Cloud

---

## 🧪 Testing

You can test the API using:

- Swagger UI
- Postman
- Insomnia

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Pavithra M**

GitHub: https://github.com/yourusername

Email: your-email@example.com

---

## ⭐ Acknowledgements

- FastAPI Documentation
- Python Documentation
- SQLite Documentation

If you found this project helpful, please consider giving it a ⭐ on GitHub!
