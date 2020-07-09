# FastDJ

This is an experiment to demonstrate one potential way of running FastAPI with Django.

The target to replace DRF with FastAPI, it makes use of a combination of Django on the model side and FastAPI on the view side, which gives you the best of both sides, Django Admin and ORM as well as FastAPI simplicity and auto-documentation.

## Setup

```
pip install -r requirements.txt
cd django_fastapi/
./manage.py migrate
./manage.py createsuperuser 
```

## Running

```
uvicorn project.asgi:app --debug --reload --port 9900
```

## Routes

The Django app is available at `/django` (e.g. `http://localhost:9900/django/admin/`

The FastAPI app is is available at `/api` (e.g. `http://localhost:9900/api/items/`