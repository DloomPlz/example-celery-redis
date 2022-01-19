Example made via https://testdriven.io/blog/flask-and-celery/

# Asynchronous Tasks with Flask and Celery

Example of how to handle background processes with Flask, Celery, and Docker.

### Quick Start

Spin up the containers:

```sh
$ docker-compose up -d --build
```

Open your browser to [http://localhost:5004](http://localhost:5004)


`docker-compose up -d --build --scale worker=3`

`curl http://localhost:5004/tasks -H "Content-Type: application/json" --data '{"type": 1}'`

`curl http://localhost:5004/tasks/TASK_ID_TOCHANGE`

