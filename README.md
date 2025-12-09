# ALX Travel App

A Django-based travel listing platform with REST API and Swagger documentation.

## Project Setup

### Prerequisites
- Python 3.8+
- MySQL 5.7+
- pip

### Installation

1. Clone the repository:
```bash
git clone https://github.com/M-Wonder/alx_travel_app.git
cd alx_travel_app
```

2. Create virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Create `.env` file with your database credentials:
```env
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_NAME=alx_travel_app_db
DATABASE_USER=your_mysql_user
DATABASE_PASSWORD=your_mysql_password
DATABASE_HOST=localhost
DATABASE_PORT=3306
```

5. Create MySQL database:
```bash
mysql -u root -p
CREATE DATABASE alx_travel_app_db;
EXIT;
```

6. Run migrations:
```bash
python manage.py makemigrations
python manage.py migrate
```

7. Create superuser:
```bash
python manage.py createsuperuser
```

8. Run the development server:
```bash
python manage.py runserver
```

### API Documentation
- Swagger UI: http://127.0.0.1:8000/swagger/
- ReDoc: http://127.0.0.1:8000/redoc/
- Admin Panel: http://127.0.0.1:8000/admin/

## Project Structure
```
alx_travel_app/
├── alx_travel_app/      # Project configuration
├── listings/             # Listings app
├── manage.py
├── requirements.txt
└── .env (not in git)
```

## Technologies Used
- Django 4.2+
- Django REST Framework
- MySQL
- Swagger (drf-yasg)
- Celery
- Redis
