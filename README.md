# BookCatalog API

DevOps online diploma coursework — a **Django REST API** project for managing a book catalogue.

## Project Structure

```
Devops_test/
├── manage.py                 # Django CLI entry point
├── bookcatalog/              # Django project configuration
│   ├── __init__.py
│   ├── asgi.py               # ASGI config for async serving
│   ├── settings.py           # Main settings (Django 4.2.30)
│   ├── urls.py               # Root URL configuration (admin + API)
│   └── wsgi.py               # WSGI config for production serving
├── api/                      # REST API app (stub)
│   ├── __init__.py
│   ├── admin.py              # Admin panel registration
│   ├── apps.py               # App config (ApiConfig)
│   ├── models.py             # Database models (to be defined)
│   ├── views.py              # API views (to be defined)
│   ├── tests.py              # Tests (to be written)
│   └── migrations/
│       └── __init__.py
├── .env/                     # Python virtual environment
├── .gitignore                # Git ignore rules
├── db.sqlite3                # SQLite database (dev)
└── README.md                 # This file
```

## Tech Stack

- **Python 3** with **Django 4.2.30**
- **Django REST Framework** (registered as `rest_framework` in INSTALLED_APPS)
- **SQLite** (development database)

## Getting Started

```bash
# Activate the virtual environment
source .env/bin/activate

# Run the development server
python manage.py runserver

# Apply database migrations
python manage.py migrate

# Create a superuser for the admin panel
python manage.py createsuperuser
```

## API Endpoints

- `/admin/` — Django admin interface
- Additional REST endpoints will be added as the API app is developed

## Development Status

The project is in its early stages. The `api` app is scaffolded with Django REST Framework integrated but no models, serializers, or views have been implemented yet.
