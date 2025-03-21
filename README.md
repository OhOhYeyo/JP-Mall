# JP-Mall
django, python, REST-ful API, BackEnd Server


# 가상환경 접근
python3.13 -m venv django-env

.\venv\Scripts\activate

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

pip install -r requirements.txt

django-admin startproject config .

python3 manage.py runserver 0.0.0.0:8000

python manage.py collectstatic
python manage.py makemigrations
python manage.py migrate

python manage.py runserver
python manage.py startapp accounts
# config settings.py accounts add
python manage.py createsuperuser