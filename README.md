# README

First, install [docker](https://www.docker.com/community-edition) and [docker-compose](https://docs.docker.com/compose/install/)

Then run these commands to build your docker image and run the app.

```
docker-compose build
docker-compose up
docker-compose run app rake db:create
docker-compose run app rake db:migrate
```

To check whether your container is running, and get the ID of the container, run the command `docker ps`.

To access the command line of your docker container running rails, use the following command:

```
docker-compose exec app /bin/bash
```

This will put you on a linux commandline within your container. Any rails commands you find in documentation you want to run from here.
