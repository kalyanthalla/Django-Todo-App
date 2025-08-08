# 📝 Django To-Do Application

![Django](https://img.shields.io/badge/Django-3.2-green)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey)

A full-featured task management web application built with Django, including user authentication and CRUD operations, designed with a responsive Bootstrap UI and ready for production deployment.

---

## 🚀 Features

- ✅ User Authentication (Login / Logout)
- 📝 Task CRUD (Create, Read, Update, Delete)
- 🔒 User-Specific Task Management
- 🎨 Responsive UI using Bootstrap
- ⚙️ Production-Ready Configuration

---

## 📦 Prerequisites

- Python 3.8+
- Django 3.2+
- pip (Python package manager)

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

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the Database

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

- App: http://localhost:8000  
- Admin Panel: http://localhost:8000/admin

---

## 🗂️ Project Structure

```
django-todo-app/
├── todoproject/          # Project configuration
│   ├── settings.py       # Django settings
│   └── urls.py           # Project-level URLs
├── todo/                 # Todo application
│   ├── models.py         # Task model
│   ├── views.py          # View logic
│   ├── urls.py           # App URLs
│   └── templates/        # App-specific templates
├── templates/            # Base templates
├── db.sqlite3            # SQLite database (development)
└── manage.py             # Django CLI entry point
```

---

## 🛠️ Configuration

In `todoproject/settings.py`:

```python
# Important production settings
DEBUG = False
ALLOWED_HOSTS = ['yourdomain.com', 'localhost']
```

---

## 🚢 Deployment (Production)

For deploying the app to production:

1. **Use PostgreSQL instead of SQLite**
2. **Set environment variables for security (e.g., SECRET_KEY)**
3. **Use a production server stack (e.g., Gunicorn + Nginx)**

### Install Production Packages

```bash
pip install gunicorn psycopg2-binary
```

---

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository
2. Create a new feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m "Add new feature"`
4. Push to the branch: `git push origin feature-name`
5. Open a pull request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

**Happy Task Managing!** ✨
