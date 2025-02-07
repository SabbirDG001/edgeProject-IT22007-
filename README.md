# Django Project- Virtual Judge

This repository contains a sample Django project with all required files and setup instructions.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository_url>
cd my_django_project
```

### 2. Create a Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use: .\venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Database Settings (Optional)
Update the `DATABASES` section in `my_django_project/settings.py` if necessary.

### 5. Run Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create a Superuser
```bash
python manage.py createsuperuser
```

### 7. Run the Server
```bash
python manage.py runserver
```
Visit [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.

## Deployment Notes
- Ensure all sensitive information is stored in environment variables and not hardcoded in the project files.
- Recommended: Use `python-decouple` for environment variable management.

## Sample Requirements File
```
Django==4.1.7
python-decouple==3.6
```

## .gitignore File
```
*.pyc
__pycache__/
db.sqlite3
.env
venv/
*/migrations/
