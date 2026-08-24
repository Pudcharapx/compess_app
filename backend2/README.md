# backend2

OpenID Connect provider built with `django-oidc-provider`.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py creatersakey
python manage.py runserver 8001
```

Configure an OIDC client in `/admin/` and inspect discovery at `/oidc/.well-known/openid-configuration`.
