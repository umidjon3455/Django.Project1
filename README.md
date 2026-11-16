# Django.Project1

Django 5.2 starter project. Python 3.11 or newer is recommended.

## Setup (Windows PowerShell)

```powershell
py -3.11 -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
Copy-Item .env.example .env
```

Open `.env` and replace `DJANGO_SECRET_KEY` with a unique secret value.

Then run:

```powershell
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Open http://127.0.0.1:8000/ and the admin panel at
http://127.0.0.1:8000/admin/.

## Environment variables

- `DJANGO_SECRET_KEY`: required secret key; never commit the real value.
- `DJANGO_DEBUG`: use `True` only for local development.
- `DJANGO_ALLOWED_HOSTS`: comma-separated hostnames.

The repository currently contains only the Django project configuration;
add your Django apps and their migrations as needed.
