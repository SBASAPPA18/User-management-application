# User Management Application

## Project Overview

A comprehensive user management application built with Python, featuring backend functionality for user registration, and management.

## 1. Create Virtual Environment

python -m venv venv
venv\Scripts\activate

# 2. Install Dependencies

pip install -r requirements.txt

# 3. configure PostgreSQL

# Login to PostgreSQL

psql -U postgres

# Create Database

CREATE DATABASE mydb;

# 4. Update Database Configuration Edit (database.py)

DB_USER = "postgres"  
DB_PASSWORD = "Sharana"  
DB_HOST = "localhost"
DB_NAME = "mydb"

update above details according to your database password and user and database name.

## Running The Apllication.

cd user_management_app
uvicorn backend.main:app --reload

Backend will run on: http://localhost:8000

# Start Frontend.

open index.html file ,
Right click and click on - open with live server.

# API Endpoints

GET /users/: List all users
POST /users/: Create new user
GET /users/{id}: Get user by ID
PUT /users/{id}: Update user
DELETE /users/{id}: Delete user

# Backend API Documentation

Access Swagger UI documentation at:
http://localhost:8000/docs

# Features.

Create new users
View list of users
Update existing users
Delete users
Form validation
Responsive design
