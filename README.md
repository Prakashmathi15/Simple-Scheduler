# Simple Scheduler - Backend (FastAPI)

This is the complete backend API for the Clustrex Full-Stack Development Assignment. It provides a secure, role-based REST API for booking appointments.

The entire API is fully documented and testable using the auto-generated SwaggerUI.

# Features

Authentication: Full JWT (JSON Web Token) login and registration.

Security: Passwords are hashed using bcrypt.

Role-Based Access: A full distinction between Admin (can create slots) and User (can book) roles.

Database: Uses SQLite for fast, file-based storage.

Error Handling: Prevents double-booking at the database level.

CORS: Fully configured to work with the React frontend on localhost:3000.

# How to Run

Prerequisite: Python 3.10+

Create Virtual Environment:
``python
python -m venv venv
```

Activate Environment:

Windows: .\venv\Scripts\Activate

Mac/Linux: source venv/bin/activate

Install Dependencies:
```
pip install -r requirements.txt
```

Run the Server:
```
uvicorn main:app --reload
```

The server will be live at
```http://127.0.0.1:8000.```

Test the API

The easiest way to test all functionality is to use the built-in SwaggerUI documentation.

Once the server is running, open this URL in your browser:
http://127.0.0.1:8000/docs

You can register users, log in, create slots (as an admin), and book appointments (as a user) all from this interactive page.
