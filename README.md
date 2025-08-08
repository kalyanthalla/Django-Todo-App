# 📝 Django To-Do Application

![Django](https://img.shields.io/badge/Django-5.0-green)
![Python](https://img.shields.io/badge/Python-3.13%2B-blue)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey)

A complete task management system with user authentication, built with Django and Bootstrap.

---

## 🚀 Features

- 🔐 User Authentication (Login/Logout)
- ✅ Task Management (Create, Complete, Delete)
- 📌 User-Specific Task Isolation
- 🎨 Clean Bootstrap Interface
- ⚡ Production-Ready Configuration

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/kalyanthalla/django-todo-app.git
cd todoproject
```

### 2. Set Up a Virtual Environment

```bash
# Linux / Mac
python -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate
```

### 3. Install Requirements

```bash
pip install django
```

### 4. Run Migrations

```bash
python manage.py migrate
```

### 5. Create a Superuser (Admin)

```bash
python manage.py createsuperuser
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

Then visit:

- App: http://127.0.0.1:8000 
- Admin Panel: http://127.0.0.1:8000/admin

---

## 🗂️ Project Structure

```
todoproject/
├── todo/                 # Main app
│   ├── migrations/       # Database migrations
│   ├── templates/        # App templates
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py          # Task form
│   ├── models.py         # Task model
│   ├── urls.py           # App URLs
│   └── views.py          # View logic
├── todoproject/          # Project config
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py       # Django settings
│   ├── urls.py           # Main URLs
│   └── wsgi.py
├── templates/            # Base templates
│   ├── base.html         # Main template
│   └── registration/     # Auth templates
│       └── login.html
├── db.sqlite3            # Development database
└── manage.py             # Command utility
```

---

## 🛠️ Configuration

In `todoproject/settings.py`:

```python
DEBUG = True  # Set to False in production
ALLOWED_HOSTS = ['localhost', '127.0.0.1']
LOGIN_URL = 'login'
LOGIN_REDIRECT_URL = 'task_list'
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

**Happy Task Managing!** ✨
