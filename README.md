# Task Management REST API

A backend REST API for managing tasks, built with **Django** and **Django REST Framework**.  
This project demonstrates clean API design, JWT-based authentication, and basic task workflow management.

---

## 📌 Overview

This API allows users to create, update, and manage tasks securely.  
It was built as a practical backend project to apply Django REST Framework concepts such as serializers, viewsets, authentication, and CRUD operations.

---

## 🚀 Features

- RESTful API endpoints for task management
- JWT authentication (login & protected routes)
- Create, read, update, and delete tasks
- Task status management (pending / completed)
- API testing using Postman
- Clean project structure following DRF best practices

---

## 🛠 Tech Stack

- **Backend:** Django, Django REST Framework
- **Authentication:** JWT (Simple JWT)
- **Database:** SQLite (development)
- **Tools:** Postman, Git, GitHub

---

## 🔐 Authentication

This project uses **JWT authentication**.

- Users must log in to obtain an access token
- Protected endpoints require a valid JWT token
- Tokens are sent via the `Authorization` header

Example:
Authorization: Bearer <your_acces"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNzY3NzY4MDA2LCJpYXQiOjE3Njc3NjQ0MDYsImp0aSI6ImIwZmVmYzliNGU5ZTRkNmVhNjFiM2I1OThlZWIzYTNmIiwidXNlcl9pZCI6IjEifQ.PiZFuZFtN5Sst1-3oKms10EKK1V5KGvEPxKu1nSM0w4"s_token>

yaml

---

## 📂 API Endpoints (Sample)

| Method | Endpoint        | Description            |
|------|-----------------|------------------------|
| POST | /api/login/     | User login             |
| GET  | /api/tasks/     | List all tasks         |
| POST | /api/tasks/     | Create a new task      |
| PUT  | /api/tasks/{id}/| Update a task          |
| DELETE | /api/tasks/{id}/ | Delete a task       |

---

## ⚙️ Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/rabbiajams haidofficial/django-task-management-api.git
cd django-task-management-api
Create and activate virtual environment:

bash
python -m venv env
source env/bin/activate   # Windows: env\Scripts\activate
Install dependencies:

bash
pip install -r requirements.txt
Run migrations:

bash
python manage.py migrate
Start the server:

bash
python manage.py runserver
