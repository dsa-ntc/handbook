# NTC Handbook

This README should lay technical tasks like how to build the handbook
frontend locally. This README is not part of the handbook, it's part
of the frontend build process.

## Editing the handbook via GitHub

In GitHub, navigate to the file you want to edit and click the edit button.

Click "Commit changes...".

Click "Commit changes".

## Running mkdocs locally

To develop on our handbook (everything in [/docs](./docs)), it's best to use
Docker.  But if not, it's also possible to use a virtual environment.

```shell
docker build -t handbook:latest .
```

Run a live session locally.

```shell
docker run --rm -it -p 8000:8000 -v ${PWD}:/app handbook
```

### Without Docker

Create a virtual environment and activate it.

```shell
python3 -m venv venv
source vent/bin/activate
```

pip install the same plugins listed in the Dockerfile.

```shell
mkdocs serve
```
