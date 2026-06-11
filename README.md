# Patient Management System API

A REST API built with FastAPI and Python to manage patient records.

## Features
- Add, view, update and delete patient records
- BMI and health verdict calculated automatically
- Sort patients by height, weight or BMI
- Input validation using Pydantic models

## Tech Stack
- Python
- FastAPI
- Pydantic

## Setup & Run

1. Create virtual environment:
python -m venv myenv
myenv\Scripts\activate

2. Install dependencies:
pip install fastapi uvicorn

3. Run the server:
uvicorn app:app --reload

4. Open API docs:
http://127.0.0.1:8000/docs

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Welcome message |
| GET | /view | View all patients |
| GET | /patient/{id} | View single patient |
| GET | /sort | Sort patients |
| POST | /create | Add new patient |
| PUT | /edit/{id} | Update patient |
| DELETE | /delete/{id} | Delete patient |