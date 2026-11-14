# VUA ServiceDesk

VUA ServiceDesk is a web-based maintenance request management system designed to help users report, manage, and track maintenance issues.

The project is being developed as part of a software engineering project, with Django handling the backend and MySQL serving as the primary database.

## Technologies Used

- Python
- Django 5.2.19
- MySQL
- mysqlclient
- django-environ
- Git and GitHub

## Project Structure

    sen305-service-platform/
    ├── backend/
    │   ├── config/
    │   ├── core/
    │   ├── requests_app/
    │   │   └── migrations/
    │   ├── .env.example
    │   ├── manage.py
    │   └── requirements.txt
    ├── docs/
    ├── frontend/
    ├── infrastructure/
    ├── .gitignore
    └── README.md

## Features and Development

- Maintenance request management
- Service request categories and workflow information
- Request priority and status tracking
- Due-date management
- Resolution summaries
- Django administration integration
- MySQL database integration
- Database migrations and model testing

## Getting Started

### 1. Clone the repository

    git clone <repository-url>
    cd sen305-service-platform

### 2. Activate the virtual environment

    python3 -m venv .venv
    source .venv/bin/activate

### 3. Install dependencies

    cd backend
    pip install -r requirements.txt

### 4. Configure environment variables

Create a local .env file using .env.example as a template.

    cp .env.example .env

Update the environment variables with your local MySQL database credentials and a secure Django secret key.

### 5. Run database migrations

    python manage.py migrate

### 6. Start the development server

    python manage.py runserver

Open http://127.0.0.1:8000/ in your browser.

## Database

The project uses MySQL as its primary database.

Database credentials and application secrets are managed through environment variables rather than being hardcoded into the application.

## Security

- Environment files containing credentials are excluded from Git.
- Python cache files and local database files are excluded from version control.
- A .env.example template is provided for configuration.

## Development Status

The project is under active development. Backend configuration, MySQL integration, service request models, database migrations, and initial testing are being implemented.