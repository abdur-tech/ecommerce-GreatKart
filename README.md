# ecommerce-GreatKart

This is a dummy e-commerce application built using Django, designed to demonstrate basic functionalities such as user authentication, product catalog management, and order processing.

## Features

- User login and registration
- Product listing and details
- Shopping cart functionality
- Order management system

## Prerequisites

- Python 3.9.2
- PostgreSQL (optional if using a different database)


## Installation

1. **Clone the repository:**


   git clone https://github.com/abdur-tech/ecommerce-GreatKart.git
   cd ecommerce-GreatKart

## Create a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

## Install the dependencies:

cd greatkart
pip install -r requirement.txt

## Create a .env file:

n the root of the Django directory where manage.py is located, create a .env file and add the following content:

SECRET_KEY='your-secret-key'
DEBUG=True
# Email settings
EMAIL_HOST=smtp.gmail.com 
EMAIL_PORT=587
EMAIL_HOST_USER='your-email@gmail.com'
EMAIL_HOST_PASSWORD='your-email-password'
EMAIL_USE_TLS=Yes

## EMAIL configuration

Use an App Password (https://support.google.com/accounts/answer/185833?hl=en) for 'EMAIL_HOST_PASSWORD' instead of normal login password

## Set up the database:

If you're using PostgreSQL, ensure it's running and create a database for the project. Update the DATABASES setting in settings.py with your credentials.

## Apply migrations:

python manage.py migration
python manage.py migrate

## Create a superuser:

python manage.py createsuperuser

## Run the development server:

python manage.py runserver

Open your browser and navigate to http://127.0.0.1:8000/ to see the application.
