para crear el archivo de manera local necesita estar dentro del aplicativo, en motoparts
Use los siguiente comandos para construir los contenedores:

$ docker-compose up -d --build
$ docker-compose exec web python manage.py migrate
$ docker-compose exec web python manage.py makemigrations
$ docker-compose exec web python manage.py createsuperuser
