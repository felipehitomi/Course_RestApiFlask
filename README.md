# Course_RestApiFlask
Repo for the code generated on the Rest Api with Flask

Link of the course - https://www.udemy.com/course/rest-api-flask-and-python

## Utilized commands

Creating an virtual env in python

```bash
python3.10 -m venv .env
```

You need to tell the visual code studio which env use with cmd(control) + shift + p and type select interpreter

Install flask

```bash
pip install flask
```

Run flask

```bash
flask run
```

## Testing the api

Using postman

## Docker

### Build

`docker build -t rest-apis-flask-python .`

### Run

Background

`docker run -d -p 5000:5000 rest-apis-flask-python`

Terminal

`docker run -p 5000:5000 rest-apis-flask-python`

## Docker-Compose

### Run

`docker compose up`

### Recreate

`docker compose up --build --force-recreate --no-deps web`

Change the last name for the service you want

## Debug

You need to have another compose with debug command and say to vscode connect remotely to the container on certain port

`docker compose -f docker-compose.yaml -f docker-compose.debug.yaml up`