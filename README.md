# webdebugger

This webb app show HTTP headers and other useful information


## Development

### Requirements

First, you must have `make` installed, to simplify all the operations.
If you haven't, see [Makefile](Makefile) for corresponding commands.

Then, you must have `poetry` installed. See https://python-poetry.org/docs/

Or just run 
```shell
make install_poetry
```

After that, install dependencies
```shell
make requirements
```
or
```shell
poetry install --local
```

### Run tests

```shell
make pytest
```
or
```shell
poetry run pytest -v
```

## Run in docker container

### Run with docker-compose

- `docker-compose up`

App will be available on you'r IP port `80`

### Variables (`make` args)

- `APP_PORT` app listen port and container port to expose
- `APP_DELAY` delay, in seconds, before render web page

### Commands (`make` targets)

Build image
```shell
make build
```

Build image and run tests
```shell
make docker-pytest
```

Run container
```shell
make docker-run
```

Run shell inside container
```shell
make docker-shell
```

## Author

Aleksey Koloskov <vsyscoder@gmail.com>
