# Docker Vite Project

## How to run this application using docker

Install [Docker](https://docs.docker.com/get-docker/) on your machine

create a `.env` file with the content

```.env
VITE_TITLE=Docker
```

### Build and start the application

```bash
docker build -t sample-app .
docker run --rm -it -p 5173:5173 --env-file=.env sample-app
```

or using docker compose

```bash
docker compose up
```

When started, it should be accessible via http://localhost:5173
