Overview

Job Tracker is a backend application built with Django and Django REST Framework (DRF) for managing job listings and applications. It provides authentication, CRUD operations, and structured API endpoints.
Features

    User authentication (Register/Login)

    CRUD operations for job listings

    Apply to jobs with resume uploads

    RESTful API with Django REST Framework

    MySQL database integration

Tech Stack

    Django, Django REST Framework

    MySQL

    Token-based authentication

    Deployment-ready for AWS/GCP

Installation & Setup

    Clone the repository:

git clone https://github.com/prajwal-desai/job_tracker.git
cd job_tracker

Create and activate a virtual environment:

python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

Configure the database in settings.py:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'job_db',
        'USER': 'root',
        'PASSWORD': 'yourpassword',
        'HOST': '127.0.0.1',
        'PORT': '3306',
    }
}

Run migrations:

python manage.py makemigrations
python manage.py migrate

Start the server:

    python manage.py runserver

API Endpoints
Method	Endpoint	Description
GET	/api/jobs/	Retrieve all jobs
POST	/api/jobs/	Create a new job
GET	/api/jobs/{id}/	Retrieve a specific job
PUT	/api/jobs/{id}/	Update a job
DELETE	/api/jobs/{id}/	Delete a job
POST	/api/apply/{id}/	Apply for a job
Contributing

To contribute:

    Fork the repository

    Create a new branch (feature-branch)

    Commit changes (git commit -m "Added feature")

    Push to GitHub (git push origin feature-branch)

    Open a Pull Request

Contact

For any queries, reach out at:
Email: prajwaldesai101@gmail.com
LinkedIn: https://www.linkedin.com/in/prajwal-desai-474891236/
