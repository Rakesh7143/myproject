# Django Backend RBAC 

This project is a Django application implementing Role-Based Access Control (RBAC). It includes user registration, JWT authentication, and role-based access control features.

## Features

- User Registration
- User Login with JWT Authentication
- Role-Based Access Control
- User Info Retrieval

## Prerequisites

- Python 3.x
- Django
- Django REST Framework
- Django Simple JWT
- django-cors-headers

## Setup

### Installation

1. **Clone the repository**:
   ```sh
   git clone <repository-url>
   cd myproject

**Create and activate a virtual environment:**
- python -m venv "venv_name"
- Activate it "venv_name\Scripts\activate"

**Install dependencies:**
- pip install -r requirements.txt
**Database Setup**
-Run migrations:
    - python manage.py migrate
**Create a superuser:**
- python manage.py createsuperuser
- give username, email and password
**Running the Server**
- python manage.py runserver

2 . **to see the results use Postman app**
    **API endpoints**
    **Authentication**
    *1.Register:*
      - URL:localhost:8000/api/register/
      - Method: POST
      - JSON
      - Body:
          {
          "username":"new_user",
          "password":"password",
          "email":"user@example.com"
          }

    *2.Login:*
      - URL:localhost:8000/api/login/
      - Method: POST
      - JSON
      - Body:
          {
          "username":"user_name",
          "password":"password"
          }
          
    *3.Logout:*
      - URL:localhost:8000/api/logout/
      - Method: POST
      - JSON
      - Body:
          {
          "refresh":"your_refresh_key"
          }
          
    *4.Refresh:*
      - URL:localhost:8000/api/refresh/
      - Method: POST
      - JSON
      - Body:
          {
          "refresh":"your_refresh_key"
          }

## Django Provides Admin Dashboard 
  - localhost:8000/admin
username and password is super user name and password


This `README.md` file provides a comprehensive guide for setting up, running, and using your Django RBAC project. It includes sections for installation, configuration, running the server, and using the API endpoints, as well as details on how to contribute to the project.

Let me know if you need any further adjustments or additional information!

  


