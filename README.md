# Basic Docker web development environment

A few basic docker containers for little projects & tests.

##  Requirements

- This repo assumes you store your projects in  `~/Projects`
- [Docker](https://docs.docker.com/engine/installation/) is installed
- [Docker Compose](https://docs.docker.com/compose/install/) is installed

## Services

- PHP-FPM 7.3
- MySQL 5.7
- NGINX 1.15

## Accessing services

We're exposing NGINX and MySQL their ports, so you can just go to `http://127.0.0.1/` or `http://localhost/` from your browser and connect to MySQL from your client (eg: [Sequel Pro](https://www.sequelpro.com/)) using `127.0.0.1:3306` or `localhost:3306`.

To access MySQL from within your web applications you'll need to use `mysql` as host.

### Default MySQL credentials:

- **Username**: `docker`
- **Password**: `docker`
- **Database**: `docker`

## Installation / run

```bash
docker-compose up
```
