# FLASK API

[![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()

## Version

**v1.0.0**

## Dependencies

- python [https://www.python.org/](https://www.python.org/)
- flask: [https://flask-restful.readthedocs.io/en/latest/](https://flask-restful.readthedocs.io/en/latest/)
- mongodb: [https://www.mongodb.com/](https://www.mongodb.com/)
- docker: [https://www.docker.com/](https://www.docker.com/)

## PYTHON

### Installation

- create virtualenv `virtualenv -p python python-env`
- work on virtualenv `source python-env/bin/activate`
- install python dependencies by running `pip install -r requirements.txt`
- Generate documentation by running `apidoc -i ./app/ -o ./documentation/ -f .py`
- Install database mock data by running `python seeders/seed-<seed-name>.py`

### How to Use

- run `uwsgi app.ini` it will listen to http://localhost:8383 with authorization Header

### Testing

- run `test ?`

## DOCKER

### Installation

- build `docker-compose build`
- install pip `docker exec -ti pythonapi pip install -r requirements.txt`
- seed data `docker exec -ti pythonapi python seeders/seed-<seed-name>.py`

### How to Use

- run `docker-compose up`
- run `docker-compose start`
