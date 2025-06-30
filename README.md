# Expense Tracker API (FastAPI)
A FastAPI-based backend application to manage users, categories, and expenses with JWT authentication and SQLite support.

# 🔧 Features
- User registration with hashed passwords
- Expense CRUD
- Categories
- Analytics by category/date
- JWT-based Authentication

# 🔧 Tools Used
Python 3.10+
FastAPI
SQLModel (SQLAlchemy + Pydantic)
Uvicorn (ASGI Server)
SQLite (Default DB)
Passlib (Password hashing)
Pydantic v2 (for schema validation)

# 🚀 Installation Steps

1. Clone the Repository
git clone https://github.com/manvigargg/expense-tracker-api.git
cd expense-tracker-api

2. Install Dependencies
pip install -r requirements.txt

3. Set Up Environment Variables
cp .env.example .env
#Then open `.env` and add your database URL and secret key:
#Example:
#DATABASE_URL=sqlite:///./expense.db
#SECRET_KEY=supersecretkey123

4. Initialize the Database
python3 -m app.core.init_db

5. Run the FastAPI Server
uvicorn app.main:app --reload

# Visit: http://localhost:8000/docs for Swagger UI.
