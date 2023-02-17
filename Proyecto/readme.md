para crear el archivo de manera local necesita estar dentro del aplicativo, en motoparts
Use los siguiente comandos para construir los contenedores:
<br>
$ docker-compose up -d --build<br>
$ docker-compose exec web python manage.py migrate<br>
$ docker-compose exec web python manage.py makemigrations<br>
$ docker-compose exec web python manage.py createsuperuser<br>
