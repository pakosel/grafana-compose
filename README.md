# grafana-compose
Run grafana along with PostgreSQL using a single command. For a simplicity of use PostgreSQL and Grafana persistent volumes are mapped so stopping the environment won't clear the data

## Prerequisites
- docker
- docker-compose

## Running services
```
sudo docker-compose up -d
```

## Accessing PostgreSQL
Open `localhost:54888/browser/` and login as `postgres/postgres`

## Accessing Grafana
Open `localhost:3000` and login as `admin/admin`. To access PostgreSQL from Grafana web interface use `postgres` as a host name and `5432` port number

## Stopping services
```
sudo docker-compose down
```
