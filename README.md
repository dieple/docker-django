## Django Development With Docker Compose and Machine

Featuring:

- Docker v1.6.1
- Docker Compose v1.2.0
- Docker Machine v0.2.0

## Local development
$ docker-machine create -d virtualbox dev
$ eval "$(docker-machine env dev)"
$ docker-machine ls
then...
$ docker-compose build
$ docker-compose -d -f docker-compose-prod.yml up
#$ docker-compose run web /usr/local/bin/python create_db.py
$ docker-compose run web /usr/local/bin/python manage.py migrate
