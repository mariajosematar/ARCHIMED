# ARCHIMED Invoice Automation

## Introduction
This project aims to automate the process of sending invoices as part of the capital call to investors.

## Problem Statement
The company currently sends invoices manually using Excel files, which leads to redundancy and maintenance issues. The goal is to build a product that automates the process of generating and managing invoices.

## Setup Instructions

### Environment Setup

1. **Create and activate a virtual environment:**
    ```bash
    python3 -m venv env
    source env/bin/activate
    ```

2. **Install Django and Django REST framework:**
    ```bash
    pip install django djangorestframework
    ```

### Project Initialization

1. **Create a new Django project and app:**
    ```bash
    django-admin startproject archimed
    cd archimed
    python manage.py startapp invoices
    ```

2. **Add 'invoices' and 'rest_framework' to `INSTALLED_APPS` in `archimed/settings.py`:**
    ```python
    INSTALLED_APPS = [
        ...
        'rest_framework',
        'invoices',
    ]
    ```

### Project Structure
