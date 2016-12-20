# Basic Docker Web Dev Box

Basic docker box for little projects & tests. I base most of my docker boxes on this one.

##  Requirements

- This repo assumes you store your projects in  `~/Projects`.
- [Docker](https://docs.docker.com/engine/installation/) installed
- [Docker Compose](https://docs.docker.com/compose/install/) installed

## Services

- PHP 7
- MySQL 5.7
- NGINX 1.10

## Accessing services

We're exposing NGINX and MySQL their ports, so you can just go to `http://127.0.0.1/` or `http://localhost/` from your browser and connect to MySQL from your client (eg: [Sequel Pro](https://www.sequelpro.com/)) using `127.0.0.1:3306`. To access MySQL from within your web applications you'll need to use `mysql` as host.

### Default MySQL credentials:

- **Username**: `docker`
- **Password**: `docker`
- **Database**: `docker`

## Installation / run

```bash
docker-compose up
```
