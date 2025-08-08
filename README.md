# Django To-Do Application

![Django](https://img.shields.io/badge/Django-3.2-green)
![Python](https://img.shields.io/badge/Python-3.8+-blue)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey)

A full-featured task management application built with Django, featuring user authentication and CRUD operations.

## Features

- ✅ User authentication (Login/Logout)
- 📝 Create, Read, Update, Delete tasks
- 🔒 User-specific task management
- 🎨 Responsive Bootstrap UI
- 🚀 Ready for production deployment

## Prerequisites

- Python 3.8+
- Django 3.2+
- pip

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/django-todo-app.git
   cd django-todo-app
Set up virtual environment

bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate    # Windows
Install dependencies

bash
pip install -r requirements.txt
Configure database

bash
python manage.py migrate
Create superuser (admin)

bash
python manage.py createsuperuser
Running the Application
bash
python manage.py runserver
Then visit:

App: http://localhost:8000

Admin: http://localhost:8000/admin

Project Structure
text
django-todo-app/
├── todoproject/          # Project configuration
│   ├── settings.py       # Django settings
│   ├── urls.py          # Main URLs
├── todo/                # Todo app
│   ├── models.py        # Task model
│   ├── views.py         # View logic
│   ├── templates/       # App templates
├── templates/           # Base templates
├── db.sqlite3           # Database (dev)
└── manage.py            # Django CLI
Configuration
Edit todoproject/settings.py for:

python
# Important settings
DEBUG = False  # Set to False in production
ALLOWED_HOSTS = ['yourdomain.com', 'localhost']
Deployment
For production deployment:

Set up a proper database (PostgreSQL recommended)

Configure environment variables

Set up a web server (Nginx + Gunicorn)

Example production requirements:

bash
pip install gunicorn psycopg2-binary
Contributing
Fork the project

Create your feature branch

Commit your changes

Push to the branch

Open a pull request

License
MIT License

Happy Task Managing! ✨
