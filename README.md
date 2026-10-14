# To-Do List Application

A simple To-Do List web application built using Python and Django. This project helps users manage daily tasks through a web interface and demonstrates the fundamentals of Django development.

## Project Overview

The To-Do List application allows users to add new tasks, view existing tasks, mark tasks as completed, and delete tasks when they are no longer required.

The project uses Django for application logic and SQLite for storing task information.

## Features

- **Add Tasks:** Create new tasks using a form.
- **View Tasks:** Display saved tasks in the application.
- **Complete Tasks:** Mark tasks as completed.
- **Delete Tasks:** Remove tasks that are no longer needed.
- **Database Integration:** Store task details using SQLite.
- **Form Validation:** Use Django ModelForms to validate task input.
- **CSRF Protection:** Protect form submissions using Django's CSRF mechanism.

## Technologies Used

- Python
- Django
- SQLite
- HTML
- CSS
- Django Templates
- Django ModelForms

## Project Structure

```text
fortodo/
├── todo/
│   ├── manage.py
│   ├── db.sqlite3
│   ├── .env
│   ├── todo/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── asgi.py
│   │   └── wsgi.py
│   └── taskapp/
│       ├── migrations/
│       ├── templates/
│       │   ├── base.html
│       │   └── taskapp/
│       │       └── task_list.html
│       ├── models.py
│       ├── forms.py
│       ├── views.py
│       ├── urls.py
│       ├── admin.py
│       └── tests.py
├── evidence.txt
└── README.md
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/codershalini210/fortodo.git
```

### 2. Navigate to the Django project folder

```bash
cd fortodo/todo
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate the environment.

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
python -m pip install django python-dotenv
```

### 5. Configure environment variables

Create a `.env` file in the same directory as `manage.py`.

Add the following configuration using your own secret key and local development settings:

```env
SK=your-django-secret-key
DJANGO_ALLOWED_HOSTS=127.0.0.1,localhost
```

Do not commit real secret keys or other confidential information to GitHub.

### 6. Apply database migrations

```bash
python manage.py migrate
```

### 7. Check the project configuration

```bash
python manage.py check
```

### 8. Run the development server

```bash
python manage.py runserver
```

Open the following address in your browser:

http://127.0.0.1:8000/

## How It Works

1. The user opens the To-Do List application.
2. Django displays the task form and existing tasks.
3. The user submits a new task through the form.
4. Django validates the form and saves valid tasks to the SQLite database.
5. The user can mark a task as completed or delete it.
6. The updated task list is displayed in the browser.

## Learning Objectives

This project demonstrates practical use of:

- Django project and application structure.
- URL routing and function-based views.
- Django models and database migrations.
- ModelForms and input validation.
- CRUD operations (Create, Read, Update and Delete).
- Django templates and template inheritance.
- Environment variables and basic application security.

## Future Improvements

- Add user registration and login.
- Allow users to edit existing tasks.
- Add task priorities and due dates.
- Add search and filtering options.
- Improve the responsive user interface.
- Add automated tests for task management.
- Configure production deployment securely.

## Author

**Shalini Rathore**

GitHub: [codershalini210](https://github.com/codershalini210)

## License

This project is available for learning and educational purposes. A formal licence has not yet been specified.
