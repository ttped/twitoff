# twitoff

## Installation

Download the repo and nagivate tehre from teh command line:

```sh
git clone https://github.com/ttped/twitoff
cd twitoff
```

## Setup

Set up and activate virtual environment
```sh
py -m pipenv install
py -m pipenv shell
```

Setup the database:
```sh
FLASK_APP=web_app flask db init
#> generates app/migrations dir

# run both when changing the schema:
FLASK_APP=web_app flask db migrate
#> creates the db (with "alembic_version" table)
FLASK_APP=web_app flask db upgrade
 #> creates the specified tables
```

## Usage

```sh
FLASK_APP=web_app flask run
```
