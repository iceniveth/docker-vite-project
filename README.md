# Docker Vite Project

## How to run this application using docker

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