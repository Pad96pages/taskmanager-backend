# Task Manager App - Django Backend

This is the backend of the Task Manager web application built with **Django** and **Django REST Framework**. It provides a RESTful API that supports user authentication and task management.

---

## ✅ Features

- User registration (custom view)
- JWT login and token refresh (via SimpleJWT)
- Authenticated CRUD operations for tasks
- Each user can manage their own tasks
- Designed to work with a React frontend

---

## 🛠 Technologies Used

- Python
- Django
- Django REST Framework
- Simple JWT (authentication)
- SQLite (default, can use PostgreSQL in prod)
- CORS Headers (for frontend connection)

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Pad96pages/taskmanager-backend.git
cd taskmanager-backend
```

### 2. Create a virtual environment
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

### 3. Install dependencies
pip install -r requirements.txt

If you don’t have a requirements.txt, you can run:
pip install django djangorestframework djangorestframework-simplejwt django-cors-headers

### 4. Run migrations
python manage.py makemigrations
python manage.py migrate

### 5. Start the server
python manage.py runserver

Test the backend using POSTMAN 
POST, GET, PUT, DELETE

### CORS Setup (for React)
In settings.py:
INSTALLED_APPS = [
    ...
    'corsheaders',
    ...
]

MIDDLEWARE = [
    'corsheaders.middleware.CorsMiddleware',
    ...
]

CORS_ALLOW_ALL_ORIGINS = True

### Frontend Repository
https://github.com/Pad96pages/taskmanager-frontend

Have a good time!

