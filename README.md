# OctoberCMS + Docker
## Development Stack

OctoberCMS is a great CMS framework built on top of Laravel. You can learn more about OctoberCMS here: https://octobercms.com/features

### System requirements:
Docker and docker-compose must be installed in order to run the stack.

### How to run the stack:

Running the stack for the first time:
```sh
$ git clone https://github.com/mbuella/octobercms-docker.git myoctoberapp
$ cd myoctoberapp
$ cp .env.docker .env
$ export APACHE_UID=$(id -u)
$ export APACHE_GID=$(id -g)
$ docker-compose up -d
```
Accessing shell inside the web container
```sh
$ docker exec -it october_app /bin/bash
```
Stopping the stack:
```sh
$ docker-compose down
```
