# Geo Django Project

A boilerplate Django project configured with PostgreSQL and environment variables.

## Setup

1. Create a virtual environment and activate it:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your database credentials
```

4. Set up PostgreSQL database:
- Create a database named `geo_db` (or your chosen name)
- Update DATABASE_URL in .env with your credentials

5. Run migrations:
```bash
python manage.py migrate
```

6. Create a superuser:
```bash
python manage.py createsuperuser
```

7. Run the development server:
```bash
python manage.py runserver
```

## Project Structure

- `geo/` - Main project configuration
- `core/` - Core Django app
- `.env` - Environment variables (not in repo)
- `.env.example` - Example environment configuration
