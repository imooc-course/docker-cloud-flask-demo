# Flask Skeleton - Docker Cloud Demo

Flask starter project... https://cloud.docker.com

## Quick Start

### Basics

1. Activate a virtualenv
1. Install the requirements

### Set Environment Variables

Update *skeleton/server/config.py*, and then run:

```sh
$ export APP_SETTINGS="skeleton.server.config.DevelopmentConfig"
```

or

```sh
$ export APP_SETTINGS="skeleton.server.config.ProductionConfig"
```

### Create DB

```sh
$ python manage.py create_db
$ python manage.py db init
$ python manage.py db migrate
$ python manage.py create_admin
$ python manage.py create_data
```

### Run the Application

```sh
$ python manage.py runserver
```

So access the application at the address [http://localhost:5000/](http://localhost:5000/)

> Want to specify a different port?

> ```sh
> $ python manage.py runserver -h 0.0.0.0 -p 8080
> ```

### Testing1

```
$ tox
```

## Docker

```
docker run -d -p 8080:5000 imooc-course/docker-cloud-demo:latest
```
