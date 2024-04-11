# useful commands (in terminal)
- docker-compose up -d --build
> creates docker container and sets app described in docker-compose and Dockerfile files

- docker-compose exec [name of app in docker-compose]
> ex: docker-compose exec web python manage.py runserver

# setting order
1) create Dockerfile on manage.py level
2) create entrypoint.sh on manage.py level
> need to be LF not CRLF
3) create docker-compose on previous level
4) run command "docker-compose up -d --build"