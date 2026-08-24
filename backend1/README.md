# backend1

Django REST API with JWT authentication.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver 8000
```

Token endpoints:

- `POST /api/token/` with `username` and `password`
- `POST /api/token/refresh/` with `refresh`
- `GET /api/me/` with `Authorization: Bearer <access>`
