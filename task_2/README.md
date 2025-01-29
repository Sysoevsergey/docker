docker run --env-file .env -d --name django-app -p 8000:8000 django-app:0.1

docker exec -it django-app python manage.py migrate

http://127.0.0.0:8000/api/v1/