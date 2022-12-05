# DRF Cinema API (dockerized)

## Installing using GitHub:

    cd cinema-api-docker\
    git clone https://github.com/FranchukS/drf-cinema-api.git

### install requirements
    - python -m venv venv\
    - venv\Scripts\activate (on Windows)\
    - source venv/bin/activate (on macOS or bash)\
    - pip install -r requirements.txt

### set your ENV variables
    set DB_HOST=<your db hostname>
    set DB_NAME=<your db name>
    set DB_USER=<your db username>
    set DB_PASSWORD=<vour db user password>
    set SECRET_KEY=<your secret key>

### run migrations and server
    python manage.py migrate
    python manage.py runserver

### Run with docker:
#### Docker should be installed
    docker-compose build
    docker-compose up

### Getting access:
create user via `/api/user/register/`\
get access token via /api/user/token/
### Features:
JWT authenticated\
Admin panel `/admin/`\
Documentation is located at `/api/doc/swagger/`\
Managing orders and `tickets`\
Creating movies with genres, `actors`\
Creating `cinema halls`\
Adding `movie sessions`\
Filtering movies and `movie sessions`
