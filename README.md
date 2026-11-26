## Patient Symptom Tracking Application

## Project Overview
The Patient Symptom Tracking Application is a web-based healthcare project developed using Python, FastAPI, SQLite, HTML, CSS, and JavaScript.

It allows patients to record their symptoms, provide severity levels, and maintain a timestamped history of their health records.

## Features
- Add new patient symptom records.
- Validate symptom descriptions to prevent empty entries.
- Validate symptom severity between 1 and 10.
- Store patient symptom records in an SQLite database.
- Retrieve symptom history using REST APIs.
- Display symptom records in a web dashboard.
- Sort symptom records by timestamp.
- Automated API testing using Pytest.
- Visualize symptom severity trends.

## Technologies Used
- **Programming Language:** Python
- **Backend Framework:** FastAPI
- **Database:** SQLite
- **Frontend:** HTML, CSS, JavaScript
- **API Testing:** Pytest
- **Data Validation:** Pydantic
- **ORM:** SQLAlchemy

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/symptoms` | Add a new symptom record |
| GET | `/patients/{patient_id}/symptoms` | Retrieve patient symptom history |
| GET | `/patients/{patient_id}/symptoms/trends` | Retrieve symptom severity trends |
| GET | `/health` | Check API health |

## Input Validation
- Patient ID must be provided.
- Symptom description cannot be empty.
- Severity must be between 1 and 10.

## Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/Amrita-22kumari/Patient-Symptom-Tracking-Application.git
```

### 2. Extract the project ZIP file
Extract `patient-symptom-tracker.zip` and open the project folder.

### 3. Install dependencies
```bash
pip install fastapi uvicorn sqlalchemy pydantic pytest httpx
```

### 4. Run the application
Open the project directory in the terminal and run:

```bash
cd patient-symptom-tracker/backend
uvicorn main:app --reload
```

### 5. Open the application
Visit:

- Frontend: http://127.0.0.1:8000
- API Documentation: http://127.0.0.1:8000/docs

## Run Automated Tests

From the project root directory:

```bash
pytest tests/test_api.py -v
```

## Project Objective
The objective of this project is to develop a simple and reliable patient symptom tracking system that demonstrates REST API development, input validation, database integration, and automated testing.

## Author
**Amrita Kumari**
