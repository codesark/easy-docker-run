# Easy Docker Run
Docker Compose files and Docker Commands for quickly starting most commonly used services for development use. 

## PostgreSQL + PgAdmin

- Host: localhost, postgres
- Network: postgres-net 
- Port: 5432
- UI: http://localhost:10081
- UI User: postgres@pgadmin.org | Password: postgres

### Create
```shell
docker network create postgres-net
docker run --name postgres -d -p 5432:5432 \
    --network=postgres-net \
    -e POSTGRES_PASSWORD=postgres \
    -v postgres-data:/var/lib/postgresql/data \
    postgres:latest
docker run --name pgadmin -d -p 10081:80 \
    --network=postgres-net \
    -e PGADMIN_DEFAULT_EMAIL=postgres@pgadmin.org \
    -e PGADMIN_DEFAULT_PASSWORD=postgres \
    dpage/pgadmin4
```

### Remove
```shell
docker stop postgres
docker stop pgadmin
docker rm postgres
docker rm pgadmin
docker network rm postgres-net

# Delete Volume (removes all data)
docker volume rm postgres-data
```
