# User Profile Django Project

This is a simple Django project with a one-to-one relationship between `User` and `Profile`.

## Features

- Each `User` has an associated `Profile` with:
  - Bio
  - Location
  - Birth date

- Signals automatically create and save profiles when users are created.

## Setup Instructions

### 1. Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 2. Install Django

```bash
pip install django
```

### 3. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 4. Create Superuser (Optional)

```bash
python manage.py createsuperuser
```

### 5. Run Development Server

```bash
python manage.py runserver
```

Visit `http://127.0.0.1:8000/admin` to access the admin panel.

## Push to GitHub

```bash
git init
echo "venv/" > .gitignore
echo "*.pyc" >> .gitignore
echo "__pycache__/" >> .gitignore
echo "db.sqlite3" >> .gitignore

git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/yourrepo.git
git branch -M main
git push -u origin main
```
