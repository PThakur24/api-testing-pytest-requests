# API Testing — Pytest + Requests

Automated REST API tests (CRUD) using Python `requests` + `pytest` on `jsonplaceholder.typicode.com`.

## What it tests
- GET /users → status, schema keys, response time
- POST /posts → create payload, validate response
- PUT /posts/1 → update and verify response
- DELETE /posts/1 → delete and confirm

## Run locally
```bash
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
pytest --html=reports/report.html --self-contained-html
