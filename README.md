# Django Todo Project

This is a simple **Todo web application** built with Django. It uses **SQLite** as the default database and supports basic task management features.

## Features

- Add, update, and delete tasks  
- Mark tasks as completed  
- Simple and clean UI  
- Built with Django 3.x+  
- Uses SQLite for lightweight local data storage  

## Requirements

- Python 3.6+  
- Django 3.0+  
- SQLite (comes built-in with Python)  

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/todo.git
   cd todo
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate        # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**
   ```bash
   python manage.py migrate
   ```

5. **Run the development server**
   ```bash
   python manage.py runserver
   ```

6. Open your browser and go to `http://127.0.0.1:8000/`

## Project Structure

```
todo/
├── tasks/                 # Main app handling the todo logic
├── todo/                  # Project configuration (settings, urls, wsgi/asgi)
│   ├── asgi.py
│   ├── urls.py
│   └── settings.py
├── db.sqlite3             # SQLite database file
├── manage.py
└── requirements.txt       # List of Python dependencies
```

## Default Database

This project uses **SQLite** as its default database, configured in `todo/settings.py`. It is ideal for local development and lightweight use.

## Admin Access

To access the Django admin panel:

1. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

2. Login at:
   ```
   http://127.0.0.1:8000/admin/
   ```

## Deployment Notes

For production use, consider:

- Switching to PostgreSQL or MySQL  
- Using Gunicorn + Nginx  
- Setting `DEBUG = False` in `settings.py`  
- Properly serving static files  

## License

This project is open-source and available under the **MIT License**.
