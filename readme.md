

This is a simple **FastAPI** REST API for managing tasks, built as part of the Webinix backend developer assessment.

---

## ✅ Features

- Create, read, update, and delete tasks (CRUD)
- Store tasks in a local **SQLite** database
- Filter tasks by `is_completed` status: `GET /tasks?is_completed=true`
- Automatic interactive API docs with **Swagger UI**
- Basic error handling (404 if a task is not found)

---

## 📂 Task Model

Each task has:
- `id`: Auto-increment integer (primary key)
- `title`: String (required)
- `description`: String (optional)
- `is_completed`: Boolean (default: `false`)

---

## ⚙️ Requirements

- **Python 3.10+**
- Recommended: create a virtual environment

---

## 📥 Installation

1️⃣ Clone this repository or download the source code.

2️⃣ Navigate into the project folder:

cd your_project_folder

3️⃣ Create a virtual environment :
python -m venv venv

4️⃣ Install dependencies:
pip install fastapi uvicorn sqlalchemy pydantic

Running the API Locally
Start the FastAPI server using uvicorn
uvicorn main:app --reload
The server will run at http://127.0.0.1:8000

Interactive API Docs
Once the server is running, open your browser and visit:

Swagger UI: http://127.0.0.1:8000/docs

---

The SQLite database file tasks.db will be created automatically when you run the server.
