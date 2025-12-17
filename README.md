# Stock-management
📦 Stock Management System

A simple Django-based stock management web application for tracking products, transactions, and inventory flow.

Overview

Stock Management System is built using Python and Django. It allows users to manage stock items, record transactions, and maintain inventory in a structured web interface. Ideal for small businesses or individuals who want to streamline stock management.

Features

User-friendly dashboard to view inventory

Add, update, and delete products

Record stock transactions

Track remaining inventory levels

Simple HTML/CSS frontend

Custom transaction history pages

Technologies Used

Python

Django

Django Templates (HTML/CSS)

SQLite

Dependencies in requirements.txt

Installation

Clone the repository

git clone https://github.com/Issa-Josiah/Stock-management.git
cd Stock-management


Create and activate a virtual environment

py -3.10 -m venv env
env\Scripts\activate


⚠ Recommended Python 3.10 for compatibility.

Install dependencies

pip install -r requirements.txt


Apply database migrations

python manage.py makemigrations
python manage.py migrate


Create superuser (optional)

python manage.py createsuperuser


Start the development server

python manage.py runserver


Open in browser: http://127.0.0.1:8000/

Configuration

Ensure the following apps are in INSTALLED_APPS:

INSTALLED_APPS = [
    ...
    'crispy_forms',
    'inventory',
    ...
]


If crispy_bootstrap4 is missing:

pip install crispy-bootstrap4


And in settings:

CRISPY_ALLOWED_TEMPLATE_PACKS = "bootstrap4"
CRISPY_TEMPLATE_PACK = "bootstrap4"

Project Structure
Stock-management/
│── inventory/                  # Inventory app
│── core/                       # Django project files
│── manage.py
│── db.sqlite3
│── requirements.txt
│── README.md

Notes

Built with Django 3.0.7, Python 3.10 recommended

Python 3.14 may produce errors with some old dependencies

Contributing

Fork the repo

Create a new branch

Make changes

Open a Pull Request

License

(Add your license here, e.g., MIT, GPL, etc.)
